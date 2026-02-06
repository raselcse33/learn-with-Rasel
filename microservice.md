<h1 align="center">Hi 👋, I'm Rasel Munshi</h1>
<h3 align="center">A Passionate Fullstack Developer from Bangladesh</h3>

# Microservice 

## Microservice + Gateway context এ final picture

```
Frontend
   |
   |  http://192.168.68.101:6692/api/v1
   v
Nginx Gateway (6692:80) [Host/pc port : 6692 and Ninx port : 80]
   |
   | route by path
   |
   ├── /scheme → (Nginx (5001 : 80)) -> scheme-service
   ├── /user   → (Nginx (5002 : 80)) -> user-service
   └── /auth   → (Nginx (5003 : 80)) -> auth-service
```
## এইটা মুখস্থ
```
User
 → Gateway (80)
 → Service Nginx (80)
 → App (9000 / internal)
 → DB
```
1.Container এর ভিতরে nginx সাধারণত 80 এ শোনে .
2.PHP container → php-fpm runs on 9000

এই port:
❌ browser থেকে access হয় না
❌ docker ports দিয়ে expose করা হয় না
✅ শুধু service nginx → php-fpm ব্যবহার করে


## একটা লারাভেল প্রজেক্ট docker করতে গেলে সাধারণত ৩ টা container লাগে। 

```
1. App (Laravel / Node / Java)
2. Nginx (reverse proxy)
3. Database
```
আমার এই প্রজেক্ট ৪ টা আছে 
```
| Container                   | কাজ     |
| --------------------------- | ------- |
| mochta_scheme_service       | PHP app |
| mochta_scheme_service_nginx | nginx   |
| mochta_scheme_service_db    | mysql   |
  phpMyAdmin = optional
```
1.PHP app container public port expose করে না,
কিন্তু internally php-fpm 9000 port এ শোনে।

2.Nginx: হলো এই app নিজস্ব সার্ভার যেটা আমার php কোড কে রান করে। এর পোর্ট হল 5001 (ইচ্ছা মত দেয়া যায়। ) যেমন আমরা 
php artisan serve --port=8001 এই কম্যান্ড টা ব্যবহার করি,
আমাদের মত port সেট করে লারাভেল প্রজেক্ট রান করি.

example:
```
 mochta_scheme_service_nginx:
    image: nginx:alpine
    container_name: mochta_scheme_service_nginx
    restart: unless-stopped
    tty: true
    ports:
      - "5001:80"
      - "5431:443"
    volumes:
      - ./:/var/www
      - ./.docker/nginx/conf.d/:/etc/nginx/conf.d/
    networks:
      - mochta_scheme_service_network
  # phpmyadmin service
  mochta_scheme_service_phpmyadmin:
    image: phpmyadmin/phpmyadmin
    restart: unless-stopped
    container_name: mochta_scheme_service_phpmyadmin
    depends_on:
      - mochta_scheme_service_db
    ports:
      - "5002:80"
    environment:
      PMA_HOST: mochta_scheme_service_db
      MYSQL_ROOT_PASSWORD: ${DB_PASSWORD}
    networks:
      - mochta_scheme_service_network
```

3.Database: Database, আমার এই প্রজেক্ট mysql database ব্যবহার করা হয়েছে। এরও একটা হোস্ট এন্ড কন্টেইনার পোর্ট আছে। আমার এই প্রজেক্ট সেটা হল 
 - "33065:3306"
```
 #MySQL Service
  mochta_scheme_service_db:
    image: mysql:8.0
    container_name: mochta_scheme_service_db
    restart: unless-stopped
    ports:
      - "33065:3306"
    environment:
      MYSQL_DATABASE: ${DB_DATABASE}
      MYSQL_ROOT_PASSWORD: ${DB_PASSWORD}
      MYSQL_PASSWORD: ${DB_PASSWORD}
      MYSQL_USER: ${DB_USERNAME}
      SERVICE_TAGS: dev
      SERVICE_NAME: mysql
    volumes:
      - mochta_scheme_service_mysql_data:/var/lib/mysql
    networks:
      - mochta_scheme_service_network
```

container ভিতরে → MySQL সবসময় 3306
Host থেকে access → 33065
Laravel .env এ কিন্তু তুমি 3306 ই ব্যবহার করবে, 33065 না
(এইটা অনেকেই ভুল করে)



4.PHPMyadmin:PHPMyadmin : PHPMyadmin হল একটা web browsing টুল যার মাধমে আমরা ডাটাবেসে বিভিন্ন রকম query করতে পারি। ম্যানুয়ালি import ,export আরো অনেক কিছু করতে পারি .এর পোর্ট 5002 .
```
  mochta_scheme_service_phpmyadmin:
    image: phpmyadmin/phpmyadmin
    restart: unless-stopped
    container_name: mochta_scheme_service_phpmyadmin
    depends_on:
      - mochta_scheme_service_db
    ports:
      - "5002:80"
    environment:
      PMA_HOST: mochta_scheme_service_db
      MYSQL_ROOT_PASSWORD: ${DB_PASSWORD}
    networks:
      - mochta_scheme_service_network
```      

## Frontend থেকে যেভাবে connection হয় backend এ 

```
# API_URL="http://192.168.68.110:7891/api/v1" 
# API_URL="http://etrade.dls.gov.bd/api/v1"
# API_URL='http://118.179.149.36:7891/api/v1'
API_URL="http://192.168.68.101:6692/api/v1"

# FILE_URL="http://192.168.68.110:7891"
# FILE_URL="http://etrade.dls.gov.bd"
# FILE_URL='http://118.179.149.36:7891'
FILE_URL="http://192.168.68.101:6692"
```

### ডিটেলস
192.168.68.101
এটা হচ্ছে আমার প্রাইভেট নেটওয়ার্ক এড্রেস। 
6692 : এটা হচ্ছে আমার gateway এর হোস্ট পোর্ট ,যার মাধমে আমি এই container এর ভিতর প্রবেশ করবো (80)। 


### finally API routing (clean microservice style)

```
upstream scheme-service {
    zone api_endpoints 64k;

	#Load Balancing back-end APIs
    server mochta_scheme_service_nginx;
    # server 192.168.50.147:1003;

	# sticky cookie srv_id expires=1h;

}

location /api/v1/scheme {
    proxy_pass http://scheme-service;
}

```

```
/api/v1/scheme
 → scheme-service
 → mochta_scheme_service_nginx
 → Laravel
```





