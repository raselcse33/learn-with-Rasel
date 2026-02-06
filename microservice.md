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
Nginx Gateway এন্ড Service Nginx এদের container  port সবসময় এটাই 

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
1.PHP APP এখানে আমার php কোড থেকে। so এর কোনো পোর্ট নাই। 
2.Nginx: হলো এই app নিজস্ব সার্ভার যেটা আমার php কোড রান করে। এর পোর্ট হল 5001 (ইচ্ছা মত দেয়া যায়। ) যেমন আমরা 
php artisan serve --port=8001 এই কম্যান্ড টা ব্যবহার করে ,আমাদের মত port সেট করে লারাভেল প্রজেক্ট রান করি.

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
````

4.PHPMyadmin:PHPMyadmin : PHPMyadmin হল একটা web browsing টুল যার মাধমে আমরা ডাটাবেসে বিভিন্ন রকম query করতে পারি। ম্যানুয়ালি import ,export আরো অনেক কিছু করতে পারি .এর পোর্ট 5002 .
```
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


