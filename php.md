# PHP Topics Start

## *********** PHP Introduction *********

---

### 🟡 Scripting Language:
**স্ক্রিপ্টিং ল্যাঙ্গুয়েজ** হচ্ছে এক প্রকার প্রোগ্রামিং ল্যাঙ্গুয়েজ যেটা compilation ছাড়াই execute হয়।  
**উদাহরণ:** `PHP`, `JavaScript`

---

### 🟡 Non-Scripting Languages:
**নন স্ক্রিপ্টিং ল্যাঙ্গুয়েজ** হচ্ছে Compiled ল্যাঙ্গুয়েজ।  
এই ল্যাঙ্গুয়েজগুলোকে কম্পিউটারে রান করার পূর্বে compiled করে মেশিন ল্যাঙ্গুয়েজে (binary code) রূপান্তর করতে হয়।  
**উদাহরণ:** `C`, `C++`, `Java`

---

### 🟡 Compiled:
Compiled মানে হচ্ছে — যেখানে আমার লেখা কোডটিকে machine language-এ (binary code) রূপান্তর করা হয়,  
যাতে কম্পিউটার বুঝতে পারে এবং ঠিকভাবে রান করতে পারে।

---

### 🟡 How Scripting Language Runs:
স্ক্রিপ্টিং ল্যাঙ্গুয়েজে compiled করার প্রয়োজন পড়ে না।  
তাই এটি রান করাতে **interpreter** ব্যবহার করা হয়  
(often part of the web server, like Apache or Nginx),  
যা কোডটি লাইন বাই লাইন পড়ে machine instructions-এ রূপান্তর করে।

---

### 🟡 PHP ভার্সন চেক করার জন্য:
```php
phpversion()
```

---

### 🟡 Web Host:
ওয়েব হোস্ট হলো একটি নির্ধারিত জায়গা যেখানে ওয়েবসাইটের ফাইল রাখা হয় — অনেকটা ভাড়া করা জায়গার মতো।  
**উদাহরণ:** `Bluehost`, `HostGator`, `GoDaddy`

---

### 🟡 Web Server:
ওয়েব সার্ভার হলো একটি টুল বা সফটওয়্যার যা ওয়েবসাইট রান করতে এবং ভিজিটরদের দেখাতে সাহায্য করে।  
**উদাহরণ:** `Apache`, `Nginx`

---

### 🟡 XAMPP:
XAMPP হলো একটি সফটওয়্যার প্যাকেজ বা ম্যানেজমেন্ট টুল যা তোমার পিসিকে একটি লোকাল ওয়েব সার্ভারে পরিণত করে।

- **X**: Cross-platform (Windows, Linux, macOS)
- **A**: Apache (Web Server)
- **M**: MySQL (Database)
- **P**: PHP (Programming Language)
- **P**: Perl (অন্য একটি programming language, আজকাল কম ব্যবহৃত হয়)

---

### 🟡 Case Sensitivity:
Case Sensitivity বোঝায় uppercase ও lowercase এর পার্থক্য।

- **Case Sensitive:** `Apple` ≠ `apple` → ভিন্ন
- **Not Case Sensitive:** `Apple` = `apple` → একি জিনিস

PHP-তে:
- **User-defined classes ও functions** → Not case sensitive
- **Built-in keywords (যেমন:** `if`, `else`, `while`, `echo`) → Case insensitive

---

### 🟡 PHP Comments:

PHP তে **comment** হচ্ছে এমন কোড বা লাইন যা রান হয় না।

**২ ধরনের কমেন্ট আছে:**

1. **Single-line comment:**  
```php
// This is a comment
# This is also a comment
```

2. **Multi-line comment:**  
```php
/*
This is a multi-line comment
It can span multiple lines
*/
```

---