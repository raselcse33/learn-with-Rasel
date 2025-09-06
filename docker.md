## Docker কী?

Docker হলো একটা কন্টেইনার প্ল্যাটফর্ম।
এটা তোমার এপ্লিকেশন + এর সব ডিপেনডেন্সি (লাইব্রেরি, কনফিগ, রানটাইম) একসাথে প্যাকেজ করে একটা ছোট “বাক্সে” (container) রাখে।
মানে —
👉 “যেকোনো মেশিনে একইভাবে অ্যাপ চালাতে চাইলে, সেটা Docker container এ চালাও।”

## কেন Docker দরকার?

Without Docker
ধরো তোমার Laravel project আছে। লোকাল মেশিনে তুমি PHP 8.2, MySQL 8, Nginx install করেছো। কিন্তু সার্ভারে যদি PHP 7.4 থাকে, project কাজ করবে না।
প্রত্যেক সার্ভারে আলাদা আলাদা ডিপেনডেন্সি install করতে হয় → ঝামেলা।

With Docker
তুমি তোমার Laravel project কে একটা Container এ রাখবে যেখানে PHP 8.2, MySQL 8, Composer, Nginx সব আগে থেকেই build করা আছে।
তখন সার্ভারে শুধু Docker install করলেই হবে → Container রান করলে project ঠিক একইভাবে কাজ করবে।

## Docker কিভাবে কাজ করে?

এটা মূলত ২টা জিনিসের উপর দাঁড়িয়ে:

### Image

একটা Image হলো template / snapshot, যেখানে তোমার অ্যাপ + dependency define করা থাকে।
Example: php:8.2-fpm, mysql:8, nginx:alpine এগুলো official Docker image।

### Container

Image থেকে Container তৈরি হয়।
Container basically হলো চলমান (running) instance of Image।
একে ভাবো, Image হলো class → Container হলো object।

## Docker এর আর্কিটেকচার (Simple flow)

তুমি একটা Dockerfile লিখবে → এখানে লিখবে:
কোন OS base হিসেবে নিবে (যেমন Ubuntu, Alpine)
কোন dependency লাগবে (PHP, Composer, MySQL)
কোন command চালাতে হবে

Docker এই Dockerfile থেকে একটা Image বানাবে।
Image থেকে তুমি এক বা একাধিক Container চালাতে পারবে।
প্রতিটি Container একে অপর থেকে isolate থাকে, কিন্তু চাইলে network এর মাধ্যমে একে অপরের সাথে connect করতে পারে।

## Docker কিভাবে Application manage করে?

ধরো তোমার একটা Laravel app আছে যেটাতে দরকার:

PHP
MySQL
Nginx

👉 Docker এ তুমি ৩টা container বানাবে:

php-container → Laravel code রান করবে

mysql-container → Database

nginx-container → Server

সবগুলোকে Docker Compose দিয়ে connect করবে (যেনো একসাথে কাজ করে)।
এখন তুমি যেখানে deploy করো না কেন (তোমার laptop, test server, production server, AWS, GCP), অ্যাপ সবসময় একইভাবে কাজ করবে।


## Dockerfile
একটি ডকারফাইল হলো একটি সাধারণ টেক্সট ফাইল, যেখানে একটি অ্যাপ্লিকেশন এবং তার পরিবেশ তৈরির জন্য প্রয়োজনীয় সব নির্দেশাবলী (instructions) লেখা থাকে। 
মানে,
কোন অপারেটিং সিস্টেম (Ubuntu/Alpine) লাগবে,
কোন সফটওয়্যার (PHP, MySQL, Node) লাগবে,
কোন ফাইল (তোমার প্রজেক্টের কোড) কপি হবে,
কোন কমান্ড রান হবে,

## Docker Image

সব মিলিয়ে সেই নির্দেশনা থেকে একটা Docker Image তৈরি হয়।
Image নিজে রান করে না। এটা শুধু “তৈরি করা snapshot/recipe”।

## Docker Container

👉 Container হলো সেই Image থেকে তৈরি রান্না করা খাবার।
Image কে ব্যবহার করে Docker একে চালু করে, একটা আলাদা ঘর (environment) বানিয়ে দেয়।
সেই ঘরে শুধু তোমার অ্যাপ্লিকেশন আর তার দরকারি জিনিস থাকবে — বাইরের কিছু মেশাবে না।
Container হলো Image-এর চলমান (running) কপি।

## উদাহরণে বোঝাই

ধরো তুমি একটা Laravel project বানাতে চাও।

তুমি একটা Image বানালে যেখানে থাকবে:

Ubuntu
PHP
Composer
তোমার Laravel code

এবার Image থেকে Container চালালে:
Container-এর ভেতরে Laravel project ঠিকমতো কাজ করবে,
বাইরের সিস্টেমে কিছু install করতে হবে না।
তুমি চাইলে একই Image থেকে একসাথে ৫টা Container চালাতে পারো। প্রতিটা আলাদা আলাদা রান করবে।

## Flow Chart (সহজ ভিজ্যুয়াল)

```
Dockerfile (নির্দেশনা লিখো)
        |
   docker build
        ↓
   Docker Image (recipe)
        |
   docker run
        ↓
Docker Container (running app)
```

## এক কথায়:

Docker Image হলো তোমার অ্যাপ্লিকেশনের প্যাকেট (code + dependency + config)।
Docker Container হলো সেই প্যাকেট থেকে চালু হওয়া অ্যাপ্লিকেশন।

