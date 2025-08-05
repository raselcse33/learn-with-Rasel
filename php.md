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

## **********Variable*********

### variable
যেখানে value assign করা থাকে 
var_dump() function এর মাধ্যমে আমরা variable টাইপ জানতে পারি .

### loosely typed language : 
PHP হল loosely typed language. এর মানে এখানে ভ্যারিয়েবল declured করার সময় বলার প্রয়জন হয় না যে ইটা কোন টাইপ এর ভ্যারিয়েবল ,
ভ্যালু দেখেই সে বুজে ফেলে যে ইটা কোন টাইপ ভ্যারিয়েবল। 
```example : $number = 5; [এর মানে এটা হলো interger টাইপ এর ভ্যারিয়েবল ] .```
```$number = "PHP " [এর মানে এটা হলো string  টাইপ এর ভ্যারিয়েবল ] .```
কিন্তু java ল্যাঙ্গুয়েজে এর ক্ষেত্রে আপনাকে vareable টাইপ declure করে দিতে হয়। 
```example :  int number = 5; [এখানে ভ্যারিয়েবল এর আগে int মানে integer কথটা বলে দেয়া হইছে ]```

### Types of Variable 
String
Integer
Float (floating point numbers - also called double)
Boolean
Array
Object
NULL
Resource   

### variable scope 
variable scope মানে হচ্ছে variable টাকে কোন কোন জায়গা থেকে access করা যাবে। কারণ সব ভ্যারিয়েবল সব জায়গা থেকে access করা যাই না। 
three main types of variable scope in PHP

### Local Scope
Local Scope হচ্ছে এই ভ্যারিয়েবল যেখানে declured করা হয়েছে শুধু ঐখানে একে এক্সেস করা যাবে আর একেই Local Scope বলে. 
এর মানে কোনো  ভ্যারিয়েবল function এর ভিতর declured করলে  কেবলমাত্র ফাঙ্কশন এর ভিতরই access করা যাবে। 
এর বাহির থেকে এক্সেস করা যাবে না .

```
function myFunction() {
$name = "John";  // Local variable, only available inside this function
echo $name;
}
myFunction();  // Outputs: John
echo $name;    // Error: $name is not accessible outside the function
```

### Global Scope 
Global Scope বা ভ্যারিয়েবল হলো,ফাঙ্কশন এর বাহিরে যে কোনো variable কে Global Scope বা Global variable বলে। 
এটা function ভিতর ছাড়া script যে কোনো জায়গা থেকে এক্সেস করা যায় 

```<?php
$name = "Alice";  // Global variable

function myFunction() {
    echo $name;  // Error: Cannot access the global variable directly inside a function
}

myFunction();  // Will produce an error
?>
```
তবে যদি আপনি ওই variable কে ফাঙ্কশন এর ভিতর থেকে এক্সেস করতে চান তাহলে global keyword use করতে হবে নিচে উদাহরণ দেয়া হলো 

```<?php
$name = "Alice";  // Global variable

function myFunction() {
    global $name;  // Use the global keyword to access the global variable
    echo $name;    // Outputs: Alice
}

myFunction();
?>
```


### Static Scope 
সাধারণত function এর ভিতর কোনো ভ্যারিয়েবল declured করলে,যখন ওই function টা রান হয় এবং শেষ হয় তখন ওই ভ্যারিয়েবল টা তার ভ্যালু delete করে দেয়। 
কিন্তু যদি variable এর আগে Static অ্যাড করা হয় তখন ওই ভ্যারিয়েবল টা, 
function শেষ হলেও ভ্যালু ডিলিট করে না। ওটা রেখে দেয়। এবং পর্বতিটিতে যখন ওই function টা কল হয় তখন ওই ভ্যারিয়েবল টা ওই ভ্যালু টা মনে রাখে।   
example
```    
<?php
function myFunction() {
    $count = 0;  // This is a regular variable
    $count++;
    echo $count;
}

myFunction();  // Outputs: 1
myFunction();  // Outputs: 1
myFunction();  // Outputs: 1
?>
```
**Simple Example without Static:
```
<?php
function myFunction() {
    $count = 0;  // This is a regular variable
    $count++;
    echo $count;
}

myFunction();  // Outputs: 1
myFunction();  // Outputs: 1
myFunction();  // Outputs: 1
?>
```
**Example with Static:  
```
?php
function myFunction() {
    static $count = 0;  // This is a static variable
    $count++;
    echo $count;
}

myFunction();  // Outputs: 1
myFunction();  // Outputs: 2
myFunction();  // Outputs: 3
?>
```

## Echo/Print

echo এবং print দুই টাই আউটপুট show করানোর জন্য ব্যবহার হয়। তবে এদের মধ্যে কিসু পার্থক্য রয়েছে। 

### echo 
echo কোনো ভ্যালু রিটার্ন করে না। এটা সিম্পলি আউটপুট শো করে। 
echo print এর থেকে ফাস্ট কারণ এটা কোনো ভ্যালু রিটার্ন করে না। 

### print 
print ভ্যালু ১ রিটার্ন করে। এবং এটা expressions এর জন্য ব্যবহার হয়।  
example 

```
<?php
if (print("Hello")) {
    echo " - The print function returned 1, so this message is shown.";
}
?>
```
এখানে print("Hello") এর মানে হলো এটা একটা স্ট্রিং hellow প্রিন্ট করছে এবং  1 ভ্যালু রিটার্ন করে কারণ আমরা জানি  প্রিন্ট সবসময় 1 রিটার্ন করে। 
যেহেতু প্রিন্ট ১ রিটার্ন করে সেহেতু condtion টা true . সেহেতু condition এর ভিতর কোড টুকু excute হবে। এখান থেকে জানা গেলো প্রিন্ট সবসময় 1 রিটার্ন করে। 
এবং এটা expressions জন্য বেবহার হয়। 
   
### why 1 is True
php তে 1 সবসময় true হিসাবে ব্যবহার  হয়। এবং 0 false হিসাবে ব্যবহার হয়। 
    example 
```
<?php
if (1) {
    echo "This will be executed because 1 is true.";
}

if (0) {
    echo "This will NOT be executed because 0 is false.";
}
?>   
```

### expressions 
expressions হলো value ,variable ,operator and function এর একটা combination যেটা একটা রেজাল্ট তৈরী  করে (সিঙ্গেল value ) .

```example : $x = 5 + 3;  // "5 + 3" is an expression that evaluates to 8 ```

Expression with Variables
```
$a = 5;
$b = 3;
$result = $a * $b;  // "$a * $b" is an expression that evaluates to 15
```

Expression with Condition

```
if (10 > 5) {
    echo "Yes";  // "10 > 5" is an expression that evaluates to true
}
```
Function Call as Expression:
```$length = strlen("Hello");  // "strlen('Hello')" is an expression that evaluates to 5```
