# PHP Topics Start

## *********** PHP Introduction *********

### ✅ Scripting Language
স্ক্রিপ্টিং ল্যাঙ্গুয়েজে হচ্ছে এক প্রকার প্রোগ্রামিং ল্যাঙ্গুয়েজে যেটা  compilation ছাড়াই execute হয়।  
**Example:**
```php
php, javascript
```

---

### ✅ Non-Scripting Languages
নন স্ক্রিপ্টিং ল্যাঙ্গুয়েজে হচ্ছে Compiled ল্যাঙ্গুয়েজ।  
মানে এই ল্যাঙ্গুয়েজ টাকে কম্পিউটার এ রান করার পূর্বে এটি কে compiled অর্থাৎ মেশিন ল্যাঙ্গুয়েজে (বাইনারি কোড এ ) রূপান্তর করতে হবে।  
**Example:**
```c
c, c++, java
```

---

### ✅ Compiled
compiled হলো সেই জায়গা যেখানে আমার লেখা কোড টাকে machine language (binary code) এ convert করা হয়,  
যাতে কম্পিউটার বুঝতে পারে এবং ঠিক ভাবে রান করতে পারে।

---

### ✅ How Scripting Language Run
যেহেতু স্ক্রিপ্টিং ল্যাঙ্গুয়েজে compiled করার প্রয়োজন পরে না,  
তাই এটা রান করার জন্য ব্যবহার করা হয় interpreter  
(often part of the web server, like Apache or Nginx)।  
এরা কোড লাইন বাই লাইন পড়ে machine instructions এর মতো করে কম্পিউটার কে বুঝায়।

---

### ✅ PHP ভার্সন চেক করার জন্য ব্যবহার করা হয়
```php
phpversion()
```

---

### ✅ Web Host
ওয়েব হোস্ট হলো একটা নির্ধারিত জায়গা যেখানে ওয়েবসাইট এর ফাইল রাখা হয় — অনেকটা ভাড়া করা জায়গার মতো।  
যেখানে যে কেউ তার মনের মত স্পেস ভাড়া নিতে পারে ওয়েবসাইট এর জন্য।  
**Example:**  
```txt
Bluehost, HostGator, GoDaddy
```

---

### ✅ Web Server
ওয়েব সার্ভার হলো একটা টুল (tool) বা software যেটা আমার ওয়েবসাইট রান করতে এবং ভিজিটরদের দেখতে সাহায্য করে।  
**Example:**  
```txt
Apache, Nginx server
```

---

### ✅ XAMPP
xammp হলো একটা সফটওয়্যার প্যাকেজ বা ম্যানেজিং টুল এর মতো যেটা আমার পিসি কে একটা লোকাল ওয়েব সার্ভার বানিয়ে ফেলতে পারি।

```txt
X: Cross-platform (works on Windows, Linux, and macOS)
A: Apache (a web server that runs your website)
M: MySQL (a database that stores your data)
P: PHP (a programming language used to build web applications)
P: Perl (another programming language, though less commonly used today)
```

---

### ✅ Case Sensitivity

**Case sensitivity** বলতে বোঝায় যে কোনো একটা লেটার বা ওয়ার্ড uppercase বা lowercase লিখলে তা একই না ভিন্ন অর্থ বোঝায়।

```txt
যেমন : Apple, apple — দুইটা কি একই না ভিন্ন?
```

- **Case sensitive:** Apple, apple → ভিন্ন
- **Not case sensitive:** Apple, apple → একই

> তবে PHP তে user define classes এবং functions এর ক্ষেত্রে এই নিয়ম মানে না।  
> যেমনঃ `if`, `else`, `while`, `echo`

---

### ✅ PHP Comment
php comment মানে এই লাইন গুলো বা কোড গুলো execute হবে না।  
php comment দুই ধরণেরঃ

**Single line comment:**
```php
// single line comment
# another single line comment
```

**Multiple line comment:**
```php
/*
This is a multi-line comment
It spans across multiple lines
*/
```