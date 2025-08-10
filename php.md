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

## PHP Data Types

### Data Type
 Data type বলতে বুঝায় ,একটা ভ্যারিয়েবল কি ধরণের  type of data (value ) hold বা ধারণ করে। 

### PHP has 8 main data types:

### String 
String হলো একটা sequence of characters (অক্ষরের ক্রম বিনাস।এর মানে হলো প্রত্যেকটা character এর পর  আরেকটা character সাজানো থাকে। 
যেমন "CAT" এখানে C A এবং T একটা সিকোয়েন্স মেইনটেইন করে একটার পর একটা রয়েছে। ) 
যেটা Double Quotes (") এবং Single Quotes (') এর ভিতর লিখা হয়।   
Characters: Letters (like A, B, C), digits (like 1, 2, 3), and symbols (like @, #, !).   
এটা লেখার জন্য single quotes (') or double quotes (") ব্যবহার করা হয়।  

### Integer
Integer বলতে বুঝায় সমস্ত নাম্বার কে (Negativ এন্ড পসিটিভ )। তবে decimal নম্বর ছাড়া।  

### Float (or Double)
Float (or Double) বলতে আমরা decimal নম্বর কে বুঝি। 

### Boolean 
Boolean হলো এক ধরণের data Type যেটা true এবং false এই দুই টা state নিয়ে কাজ করে।
true : (এর অর্থ হলো something are correct or  exit ).
False : (এর অর্থ হলো  something is incorrect or does not exist).

### When is Boolean Used?
Boolean সাধারণত ব্যবহার হয় Conditional Statements and Logical and comparison Operations এর ক্ষেত্রে। 
Conditional Statements : (like if, else) অর্থাৎ যেহেতু এটা true এবং false নিয়ে কাজ করে সেহেতু  block এর ভিতর কোড টুকু কখন  run hobe এটা নির্ধারণ করে । 
মানে যদি condtion true হয় তখন run করবে other wise করবে না। 
Logical and comparison Operations (like &&, || , > ,<) to combine or test multiple conditions.

 besic example 

 ```
<?php
$is_raining = true;   // This is a boolean value representing 'true'
$is_sunny = false;    // This is a boolean value representing 'false'

if ($is_raining) {
    echo "Take an umbrella!";  // This will run because $is_raining is true
}

if (!$is_sunny) {
    echo "It's not sunny outside.";  // This will run because $is_sunny is false
}
?>
```

Comparisons example

```
 <?php
$a = 10;
$b = 5;

$is_greater = $a > $b;  // Comparison: 10 is greater than 5, so $is_greater is true
echo $is_greater;       // Outputs: 1 (because true is displayed as 1 in PHP)

$is_equal = $a == $b;   // Comparison: 10 is not equal to 5, so $is_equal is false
echo $is_equal;         // Outputs nothing (because false is displayed as empty in PHP)
?>
```

### Type Casting 
Type Casting হলো একটা process যার মাধ্যমে value একটা data type থেকে আরেকটা data type convert হয়।    
PHP এমন অনেক ভ্যালু আছে যা automatically Booleans data কনভার্ট হয়। নিচে example দেয়া হলো : 

0 (integer zero) and 0.0 (float zero) are false.
Empty strings (""), empty arrays ([]), and null are false.
All other values (non-zero numbers, non-empty strings, non-empty arrays) are true.

```
<?php
$value1 = 0;         // 0 is false
$value2 = "Hello";   // Non-empty string is true

if ($value1) {
    echo "This is true!";
} else {
    echo "This is false!";  // Outputs this because 0 is false
}

if ($value2) {
    echo "This is true!";  // Outputs this because non-empty strings are true
}
?>
```

### Array 
Array হলো এমন একটা ভ্যারিয়েবল যেখানে  multiple ভ্যালু assign করা যায়। এবং সেই ভ্যালু গুলোকে index এর মাধ্যমে এক্সেস করা যায়।             
example 

```
<?php
$fruits = array("Apple", "Banana", "Orange");  // This is an array
echo $fruits[0];  // Outputs: Apple (first item in the array)
?>
```

### Object
Object হল instance of class . মানে হচ্ছে object হল class এর একটা বাস্তব উদাহরণ। 
যেমন car যদি একটা class হয় তাহলে এর উদাহরণ বা instance হলো Toyota .   
class : class হল একটা প্ল্যান জাস্ট plan . যেমন (car ,এর color থাকবে ,brand থাকবে একটা প্ল্যান ) .
object : object হল ঐ প্ল্যান বা class  এর একটা real উদাহরণ তৈরী করা। যেমন (car এর color রেড হবে , এবং ব্র্যান্ড টা Toyota হবে ) .
এরকম আরো multiple  উদাহরণ বা object তৈরী করা যায় একটা ক্লাস থেকে । 

```
class Car {
    public $color;
    public $model;
}

// Creating an instance of the Car class
$myCar = new Car();  // This is an instance (or object) of the Car class
$myCar->color = "Blue";
$myCar->model = "Toyota";

$myNewCar = new Car();  // multiple object 
$myNewCar->color = "red";
$myNewCar->model = "Tesla";
```

### NULL
NULL হচ্ছে  একটা special  ভ্যালু যেটা represents করে no-value অথবা empty । 
তাই কোনো ভ্যারিয়েবল কে null ভ্যালু এসাইন করা মানে হলো ঐ ভ্যারিয়েবল টা empty অথবা স্পষ্টভাবে কোনো ভ্যালু এসাইন করা নাই।
সহজ ভাবে বলতে গেলে Declaring without a value.তবে এখানে একটা কথা থাকে 

$car;
$car2 = NULL;
এখানে দুই টা ভেরিএবলে আছে যার প্রথমটা শুধু একটা ভ্যারিয়েবল declured করা আছে যার কোনো ভ্যালু নেই। 
এবং দ্বিতীয়টা একটা special null ভ্যালু assign করা আছে যার অর্থ এর ও কোনো স্পষ্টভাবে ভ্যালু এসাইন করা নাই।  তাহলে কি দুই টা একই। 

$car;
PHP জানে যে $car  কোডে উল্লেখ করা হয়েছে , কিন্তু এটা এখন ও একটা initialized variable এর মত আচরণ করে না। 
initialized variable এর মানে হলো variable টাতে intial ভ্যালু (প্রাথমিক ভাবে বা প্রথম বার যে ভ্যালু  assign করা হয়। )  
assign করা হয়েছে। মূলকথা হল $car  যেহেতু কোডে লিখা হয়েছে সেহেতু এটা exit করতেসে কিন্তু PHP একে কোনো memory allocation অর্থাৎ memory তে কোনো জায়গা বরাদ্দ রাখে না। 

$car2 = NULL
এখানে $car2 variable  একটা special ভ্যালু declured করেছে। এবং এটা  initialized ও হয়েছে  এবং memory allocation হয়েছে তবে সেটা সর্বনিন্ম। 

### Resource 
Resource হচ্ছে PHP এর একটা special ডাটা টাইপ যেটা external resource নিয়ে কাজ করে। 
external resource মানে হচ্ছে PHP Program এর বাহিরে যে কোনো data টাইপ অথবা service, যেটাকে PHP program থেকে accessed করা যাবে। 
যেমন Databases,file ,API .  
example 
```
$connection = mysqli_connect("localhost", "username", "password", "database");
এখানে $connection একটা variable যার মধ্যে database  করা হয়েছে।  
```

## PHP Strings Details

এর আগে আমরা string টাইপ নিয়ে আলোচনা হয়েছে। এখানে আমরা string এর ডিটেলস নিয়ে অলোচোনা করবো। 
আমরা জানি string টাইপ এর ডাটা বা  ভ্যালু  Double Quotes (") এবং Single Quotes (') এর ভিতর লিখা হয়। 
তবে লিখা হলেও এই Double Quotes (") এবং Single Quotes (') এর ভিতর রয়েছে পার্থক্য। 

Double Quotes : 
                     
এর প্রথম যে বৈশিষ্ট সেটা হলো Double Quotes এর ভিতর আমরা ভ্যারিয়েবল লিখতে পারি। 
এবং সেটা ভ্যারিয়েবল এর মত আচরণ করে।আর এই কথাটাকে ইংলিশ বলে (interpolated).  
একটা উদাহরণ দিলে আরো সহজ হবে। 
```
$name = "John";
echo "Hello, $name!"; // Outputs: Hello, John!
```
এটি অনেক escape sequences সাপোর্ট করে। (escape sequences হল combination  of special character) .
            
performance এর ক্ষেত্রে এটি Single Quotes এর থেকে slow  ।            
Double Quotes এর ভিতর single  Quotes লিখা যায়। 
```
echo "She said, 'Hello!' "; 
```

Single Quotes (') 
                     
এর ভিতর আমরা ভ্যারিয়েবল লিখতে পারি তবে সেটা ভ্যারিয়েবল এর মত আচরণ করে না। সে ওটাকে একটা sequence characters হিসাবে ধরে। যেমন :
```
$name = "John";
echo 'Hello, $name!';  // Outputs: Hello, $name!
```
            
এখানে লক্ষ করলে দেখা যাবে $name যে একটা ভ্যারিয়েবল এবং এর যে একটা  এসাইন কৃত ভ্যালু আছে, সে কিন্তু ওই ভ্যালু টাকে প্রিন্ট করে নাই।বরং সে নিজেই একটা sequence characters হিসাবে প্রিন্ট হয়েছে। 
            
*এটি মাত্র দুটি escape sequences সাপোর্ট করে। 
\' to include a single quote (like in It's),
\\ to include a backslash.
            
performance এর ক্ষেত্রে এটি Double Quotes এর থেকে faster । কারণ এটিতে  interpolation হয় না  এবং escape sequences কম সাপোর্ট করে। 
Single Quotes এর ভিতর Double Quotes লিখা যায়। 
```
echo 'She said, "Hello!"'; 
```
দুইটা স্ট্রিং কে  '.' দ্বারা concate করা হয়।   

## PHP Constants
আমরা জানি যার মধ্যে ভ্যালু assign করা হয় তাকে ভ্যারিয়েবল বলে। 
যেমন 
```
$name = "খেলা হবে "; 
```
এখানে $name একটা ভ্যারিয়েবল যেটা string টাইপ এর ডাটা বা ভ্যালু ধারণ করে।  
ঠিক তেমনি Constant ও হল একটা special variable যার প্রধান বৈশিষ্ট হল এর মধ্যে কোন ভ্যালু একবার ভ্যালু assign করলে এটা আর পরিবর্তন করা যায় না। 
নিচে Constant এবং variable নিয়ে আলোচনা করা হল। 

 এটা কে define() অথবা  const দিয়া শুরু করতে হয়। 
উদাহরণ 
```
 define("SITE_NAME", "MyWebsite");
 ```
এর মধ্যে একবার ভ্যালু সেট করলে সেটাকে আর changed or redefined করা যায় না । 
উদাহরণ 
```
define("PI", 3.14159); 
// Trying to change the value
PI = 3.9; // Error: Cannot reassign a value to a constant
```
এখানে যেহেতু PI এর ভ্যালু একবার সেট করা হইয়া গেছে সেহেতু আর চেঞ্জ করা যাবে না। 
```
define("GREETING", "Hello, World!"); // Define the constant GREETING
define("GREETING", "Hi, World!"); // Error: GREETING has already been defined
```
এখানে একবার GREETING define করা হয়ে গেছে সেহেতু পরে আর define করা যাবে না। দুটি উদাহরণ প্রায় একই। 
এটা uppercase letters দিয়া লিখতে হয়। 
নরমাল ভ্যারিয়েবল এর মত এর $ sign দরকার হয় না। 
PHP তে এরকম অনেক magic constant আছে। যেটা আগে থেকেই predefine করা। নিচে details দেয়া হল 
লিঙ্ক : https://www.w3schools.com/php/php_magic_constants.asp

 ## PHP Operators
PHP তে Operators বলতে বুঝায় কিছু  symbol বা keyword (keyword বলতে এখানে reserve keyword বুঝানো হয়েছে।  
যেমন if ,else ইত্যাদি  ). যেটা ব্যবহার হয় variableবা value এর উপর। বিভিন্ন রকম action  ঘটানোর জন্য। 
এখানে action বলতে বুঝানো হচ্ছে কিছু একটা করা যেমন : যোগ করা ,comapare করা ,ইত্যাদি।  

```
Arithmetic operators (+,  -,  *,  /,  %)
Assignment operators (=, += , -=, *= , /= , %=)
Comparison operators (== , === , < ,> ,!= , <= ,>= ,)
Increment/Decrement operators (++$x , $x++ ,--$x , $x--)
Logical operators(&& , ।। ,!)
String operators (. use to concate string )
Array operators (+ , == , === , != ,)
Conditional assignment operators (Ternary Operator ?:  ,  Null Coalescing Operator ?? )
Null coalescing operator : এই operator টা ব্যবহার হয় যে ভ্যারিয়েবল এর ভ্যালু আছে কিনা চেক করার জন্য। 
```

## PHP if Statements
PHP IF  statement সাধারণত ব্যবহার করা condtion চেক করার ক্ষেত্রে। condtion যখন true হয়।  
তখন ওই condition এর ভিতর code টুকু রান হয়। নিচে উদাহরন দেয়া হল 
উদাহরণ 
```
if (condition) {
    // Code to run if the condition is true
}
```
একে সংক্ষিপ্ত ভাবে ternary অপারেটর দিয়ে প্রকাশ করা যায়। মোট কথা হল ternary operator হচ্ছে if statement এর  short form যাকে shorthand if বলা হয়।
 উদাহরণ 
``` 
$variable = (condition) ? value_if_true : value_if_false;

$age = 20;
$status = ($age >= 18) ? "adult" : "minor";
echo $status; // Outputs: adult  
```
একের অধিক condition চেক করার জন্য। if elseif ব্যবহার করা হয়। switch Statement দিয়েও multiple condition check করা হয়। নিচে switch Statement উদাহরণ দেয়া হল।

উদাহরণ :
```
$fruit = "apple";
switch ($fruit) {
    case "banana":
        echo "This is a banana.";
        break;
    case "apple":
        echo "This is an apple.";
        break;
    case "orange":
        echo "This is an orange.";
        break;
    default:
        echo "Unknown fruit.";
}
```

## PHP Loop

Loop ও এক প্রকার connditional statement .এটি একটি কাজ বা বার বার করে (প্রোগ্রামিং এর ভাষায় : কোড এর একটি নির্দিষ্ট block বার বার excute করে ) 
যতক্ষণ না condtion টা false হচ্ছে। php তে চার প্রকার loop আছে , while Loop,do-while Loop,for Loop,foreach Loop

while Loop 

```
$count = 1;
while ($count <= 5) {
    echo "Count is: $count <br>";
    $count++; // Increases $count by 1 each time
}
```

do-while Loop 

```
$count = 1;
do {
    echo "Count is: $count <br>";
    $count++;
} while ($count <= 5);
```
তবে while Loop এবং do-while Loop এর মধ্যে একটা পার্থক্য আছে। সেটা হলো while Loop প্রথমে condition  check করে ,
এরপর  condtion true হলে সে ওই কোড টুকু excute করে। 
ওপর দিকে  do-while Loop প্রথমে একবার কোড excute করে then condition check করে। 

for Loop
```
for ($i = 1; $i <= 5; $i++) {
    echo "Number: $i <br>";
}
```

Step-by-Step Execution
Let's go through each iteration to see what happens.

First Iteration:

Initialization: $i = 1
Condition: $i <= 5 (true, since 1 <= 5)
Execute Code: echo "Number: 1 <br>"; // Output: Number: 1
Increment: $i++ makes $i = 2
Second Iteration:

Condition: $i <= 5 (true, since 2 <= 5)
Execute Code: echo "Number: 2 <br>"; // Output: Number: 2
Increment: $i++ makes $i = 3
Third Iteration:

Condition: $i <= 5 (true, since 3 <= 5)
Execute Code: echo "Number: 3 <br>"; // Output: Number: 3
Increment: $i++ makes $i = 4
Fourth Iteration:

Condition: $i <= 5 (true, since 4 <= 5)
Execute Code: echo "Number: 4 <br>"; // Output: Number: 4
Increment: $i++ makes $i = 5
Fifth Iteration:

Condition: $i <= 5 (true, since 5 <= 5)
Execute Code: echo "Number: 5 <br>"; // Output: Number: 5
Increment: $i++ makes $i = 6
Sixth Iteration:

Condition: $i <= 5 (false, since 6 > 5)
Since the condition is now false, the loop stops, and PHP moves on to the next part of the code.

foreach Loop : foreach Loop টা specially array ক্ষেত্রে ব্যবহার হয়। এটা দ্বারা array এর প্রতিটা এলিমেন্ট একটা একটা করে access করা যায়     
Break Statement : Break Statement টা ব্যবহার করা হয় কোনো loop কে তাৎক্ষণিক ভাবে exit বা শেষ করার জন্য,
যদিও লুপ এর condition true . একটা উদাহরণ দিলে আরো ভালো বুঝা যাবে।

```
$count = 1;
while ($count <= 10) {
    echo "Count is: $count <br>";
    if ($count == 5) {
        break; // Stop the loop when $count is 5
    }
    $count++;
}
```

এখানে while loop টা  $count  এর মান যতক্ষণ , ১০ এর থেকে ছোট বা সমান  থাকবে ততক্ষন ভিতরের কোড টুকু excute করার কথা। 
কিন্তু loop এর ভিতর আরেকটা  condition use করা হয়েছে। যখন ওই condition true হবে তখন break statement  কোড টাকে exit করে দিবে ,
যদিও loop এর condition এখনো true ।এটাই হল ব্র্যাক statement কাজ  

### Continue 
continue statement সাধারণত ব্যবহার করা হয়  কোনো একটা loop ( চক্র ) কে স্কিপ করার জন্য ।
এবং ওই loop (চক্র) কে স্কিপ করে পরবর্তী যে চক্র বা লুপ আছে ওইটা continue করে। 
কিন্তু break এর মত পুরো loop টাকে exit করে দেয় না। নিচে উদাহরণ দেয়া হল। 

```
for ($i = 1; $i <= 5; $i++) {
    if ($i == 3) {
        continue; // $i = 3 হলে এই iteration (একটি পূর্ণ চক্র ) টি স্কিপ হবে
    }
    echo "Number: $i <br>";
}
```
আউটপুট 
Number: 1
Number: 2
Number: 4
Number: 5
এখানে যখন $i  = 3 এই condition টা সত্য হয়েছে তখন ওই চক্র বা loop টিকে skip করা হয়েছে। এবং পরবর্তী যে loop বা চক্র টি আছে ঐটাকে Continue করা হয়েছে। 
[ এখানে আমি চক্র বলতে যেটা বুঝতে চেয়েছে সেটা হল। $i = 1; $i <= 5; $i++ এর মানে এখানে ৫ টা চক্র বা loop সম্পন্ন হবে কারণ condition দেয়া আছে $i <= 5; মানে $i এর 5 এর বড় হবে না। 
আমরা জানি loop মানে কোন কোড এর একটি নির্দিষ্ট block বার বার excute করে যতক্ষণ না condtion টা false হচ্ছে।  ]

## PHP Function

php function হচ্ছে code এর ভিতর একটা নির্দিষ্ট block যেটা একটা নির্দিষ্ট কাজের জন্য ব্যবহার হয়। 

[code হচ্ছে একটা instructions (নির্দেশনা) বা command যেটা কোনো programming language লেখা হয় ,
 যাতে করে কম্পিউটার ওই instructions অনুযায়ি কাজ করতে পারে (excution করতে পারে )।
আমরা জানি code লেখা হয় programming ল্যাঙ্গুয়েজে দিয়ে। প্রত্যেক single লাইন code কোনো না কোনো কাজের নির্দেশনা দেয় computer কে  যে তুমি এটা কর , 
তখন compute ওই কাজ টা করে এবং আমরা তার রেজাল্ট টা দেখতে পাই। 
মোটকথা computer এর সাথে commnucation একটা মাধ্যম হল কোড [ (programming ল্যাঙ্গুয়েজে) . 
অন্য ভাবে বললে programming language এর লিখিত রূপ হল কোড].

example

```
<?php
echo "Hello, World!";
?>
```
এখানে কোড instructions দিচ্ছে computer কে তুমি Hello, World! টেক্সট টা screen শো কর। 

function এর ব্যবহার করার অনেক গুলো উপকার আছে। 

Reusability (বার বার ব্যবহার করা যায়। )
Organization (সুগঠিত )
Maintainability (সহজে রক্ষণাবেক্ষণযোগ্যতা , যেহেতু একটা নির্দিষ্ট কাজের জন্য ব্যবহার হয়, সেহেতু খুব সহজে রক্ষণাবেক্ষণ করা যায়।একটু ডিটেলস বললে যেহেতু একটা function 
বার বার বেবহার হতে পারে কোড এর ভিন্ন ভিন্ন জায়গা থেকে , সেহেতু আমি যদি শুধু ওই function টাতে কোন পরিবর্তন আনি ,তাহলে এই পরিবর্তন সব জায়গাতেই পরবে। অর্থাৎ যারা যারা এই function call করছে।)

উদাহরণ (function):

```
<?php
function sayHello() {
    echo "Hello, World!";
}

// Calling the function
sayHello(); // Outputs: Hello, World!
?>
```
function লেখার নিয়ম হচ্ছে সাধারণত  function নাম দিযে function লেখা শুরু করতে হয়। এবং function এর একটা নাম দিতে হবে। 
sayHello হল function এর নাম এবং এর আগে function কথাটি লিখা হয়েছে । function এর ভিতরের code কে exction করতে হলে এটাকে call করতে। 
কারণ call ছাড়া এটা একা একা  exction হয় না। 

Parameters: Inputs to make functions flexible

```
function greet($name) {
    echo "Hello, $name!";
}
greet("Alice");
```
Return Values: Get results back from functions.  

```
function add($a, $b) {
    return $a + $b;
}
$sum = add(5, 3);
```
                    
Default Parameters: Provide default values for parameters

```
function greet($name = "Guest") {
    echo "Hello, $name!";
}
```

PHP বিভিন্ন ধরণের function রয়েছে নিচে আলোচনা করা হল 

User-Defined Functions : কোনো User যখন তার নির্দিষ্ট কাজের জন্য কোনো function তৈরী করে তখন তাকে User-Defined Functions বলে। 
                                 
উধাহরন

```
<?php
function greet() {
    echo "Hello, World!";
}
greet(); 
?>
```

Built-in Functions : Built-in Functions হল আগের থেকে define বা তৈরী  করা function যেটার কোনো পরিবর্তন বা modification করা যাবে না। 
শুধু ব্যবহার করা যাবে।php তে এরকম অনেক Built-in Functions রয়েছে কাজকে সহজ করার জন্য 
উধাহরন

```
echo round(4.6); // Outputs: 5
round একটা Built-in Functions যেটা সব সময় neares integer velue দেয়  
```

Anonymous Functions (Closures) : Anonymous Functions কে Closures function বলা। এই function এর কোনো নাম থাকে না। এটি সাধারণত 
ব্যবহার হয়  inline functions or assigned to variables জন্য। এবার আসি inline functions কি   
inline functions বলতে সহজে যেটা বলা যায় সেটা হল। এটি একটি ছোট function বা  temporary functions বলা যেতে পারে , 
যেটা immediately কোনো একটা কাজ সম্পন্ন করার জন্য ব্যবহার  করা হয় এবং ওরকম কোন plan থাকে না যে এটাকে আবার reuse করবো । 

example:
Inline function to square a number

```
$square = function($number) {
    return $number * $number;
};
echo $square(4); // Output: 16
```

explain: Here, $square(4) means you are calling the anonymous function stored in $square and 
passing 4 as the value for the parameter $number. ["function is stored," it means that the function is assigned to a variable.]   


assigned to variables বলতে আমরা বুজি কোনো একটা ভ্যারিয়েবল এর ভিতর ভ্যালু এসাইন করা, সিম্পল ভাবে এটাই বুজি। 
যেমন $x = "১০";
এখানে $x ভ্যারিয়েবল আর ১০ হল ভ্যালু। 
আমরা Anonymous Functions কেউ ভ্যারিয়েবল এর ভিতর এসাইন করতে পারি।     
finally আমরা বলতে পারি  ছোট এবং immediately কোনো টাস্ক সম্পন্ন করার জন্য এবং যে টাস্ক টা আমাদের বার বার use করার দরকার পরবে না। এরকম কোন কাজ করার জন্য আমাদের Anonymous Functions ব্যবহার করা হয়। এরফলে আমাদের ঘটা করে কোনো function এর নাম দিয়ে নতুন করে কোনো function লিখতে হয় না। 
ফলে এটা আমাদের কোড short হয়।     
                                        
Anonymous Functions এর আরেকটা মজার দিক রইছে।সেটা হল Local Scope . Scope নিয়ে আগে আলোচনা করা হয়েছে ,হালকা ভাবে বললে স্কোপ মানে accessible 
area . অর্থাৎ কাকে কোন কোন জায়গা থেকে access করা যাবে। Local Scope হচ্ছে এটাকে যেখানে declured করা হয়েছে শুধু ঐখানে একে এক্সেস করা যাবে। একটা 
উধাহরন দিলে সহজ হবে। 

```
$name = "Alice";
$sayHello = function() use ($name) { // Captures $name from outside
    echo "Hello, $name";
};
$sayHello(); // Output: Hello, Alice
```


এখানে $name একটা variable যেটা function এর বাহিরে declured করা হয়েছে। ফলে এটাকে  function এর ভিতর থেকে access করা যাবে না এবং access করতে গেলে একটা error দিবে . 
একে function এর বাহির থেকেই কেবল  access করতে হবে। কিন্তু Anonymous Functions  "use " কীওয়ার্ড ব্যবহার করে এই ভ্যারিয়েবল টাকে 
function এর ভিতরে ও ব্যবহার করতে পারে। মজার না। জটিল জিনিস।  

Arrow function: arrow function ও Anonymous Function এর  মতো অনেকটা। এটাও একটা inline functions,এই function এর কোনো নাম থাকে 
না ,এবং এটাকেও variable assign করা যায়, এবং দুটো function ই ব্যবহার হয় ছোট task এর জন্য। তবে এর মধ্যে কিছু পার্থক্য আছে। 
নিচে একটা উদাহরণ দেওয়া হল arrow function এর। 

```
<?php
$c = 0; // outer scope variable
$sum = fn($a, $b) => $a + $b + $c;
echo $sum(5, 10); // Output: 15  
php?> 
```

ফীচার                                    Arrow function                           

1.Syntax                              fn  keyword ব্যবহার করা হয়। 
2.Return                              এই খানে return দরকার পরে না অটোমেটিক ভাবে result return হয়। 

3.Outer Scope Variables               outer scope variable access করার জন্য কোনো keyword দরকার পরে না। অটোমেটিক ভাবেই access করা যায়। 
4.Introduced in PHP                   PHP 7.4
5.code cmplexcity                     Can not handle multiple lines of code




ফীচার                                    Anonymous Function                            

1.Syntax                              function  keyword ব্যবহার করা হয়।  
2.Return                              function এর ভিতর result পাওয়ার জন্য return  ব্যবহার করা হয়।                 

3.Outer Scope Variables               outer scope variable access করার জন্য use keyword ব্যবহার করা হয়
4.Introduced in PHP                   PHP 5.3
5.code cmplexcity                     Can  handle multiple lines of code


Recursive Functions (call) :Recursive Functions  হল এমন একটি প্রসেস, যেখানে একটি ফাঙ্কশন নিজেই নিজেকে কল করে।
একটি ফাঙ্কশন নিজেই নিজেকে পুনরায় কল করে, এবং এই প্রক্রিয়াটিকে Recursive Call বলা হয়।এবং এখানে দুটি পার্ট থাকে একটা base case (যেখানে ফাঙ্কশনটি থামবে,বা অন্য কিছু।  ) 
আরেকটা হলো recursive case (যেখানে recursion নিজেকে কল করে) 

 নিচে উদাহরণ দেয়া হলো 

```
function countdown($number) {
if ($number <= 0) { // Base case
    return;
}
echo $number . "\n"; // Print the current number
countdown($number - 1); // Recursive call
}

countdown(5);
```

## Array
Array হলো এমন একটা ভ্যারিয়েবল যেখানে  multiple ভ্যালু assign করা যায়। এবং সেই ভ্যালু গুলোকে index এর মাধ্যমে এক্সেস করা যায়। 
example

```
<?php
$fruits = array("Apple", "Banana", "Orange");  // This is an array
echo $fruits[0];  // Outputs: Apple (first item in the array)
?>
```

Type of Array:

Indexed Arrays: Arrays with numeric keys (starting from 0).
Associative Arrays: Arrays with custom string keys.
Multidimensional Arrays: Arrays containing other arrays.


Indexed Arrays : Indexed Arrays  তে  integer key ব্যবহার করা হয়। এবং এটা auto generate যদি manually assign না করা হয়। 
Example: 

```
<?php
$fruits = ["apple", "banana", "orange"]; // Indexed array

echo $fruits[0]; // Outputs: apple
echo $fruits[1]; 
?>
```

Associative Arrays : Associative Arrays তে সাধারণত string key ব্যবহার করা হয় ,তবে integer key ও ব্যবহার করা যায়, এখানে ইচ্ছা মতো কীয় ব্যবহার করা যায়।

```
$associativeArray = [
"name" => "Alice", // String key
42 => "Meaning of life", // Integer key
"city" => "Paris"
    ];
echo $associativeArray["name"]; // Outputs: Alice
echo $associativeArray[42];  
?>
```

               
main পার্থক্য টা হলো Indexed Arrays কীয় সবসময় integer ,এবং এটা auto genarate .ওপর দিকে Associative Arrays key string অথবা integer .( তবে fully customize )
USES : Indexed Arrays ব্যবহার করা  sequential data (like a list or collection) store করার জন্য. 
আর Associative Arrays বেবহার করা হয় meaningful keys সহ ডাটা store করার জন্য। 
Key  : যেহেতু array তে আমরা multiple ভ্যালু রাখি ,সেহেতু spacific ভাবে ওই ভ্যালু গুলোকে ধরার জন্য আমরা Key এর আন্ডার রাখি এটাই হলো Key .   

Multidimensional arrays : Multidimensional arrays বলতে বুঝায় যেখানে একটা array তার ভ্যালু হিসাবে array রাখে। 
আমরা জানি array এমন একটা ডাটা টাইপ বা ভ্যারিয়েবল  যেখানে  একাধিক ভ্যালু assign করা যায়। 
আর Multidimensional arrays তে ঐ ভ্যালু হিসাবে array assign করা হয়। নিচে example দেওয়া হল। 

Types of Multidimensional Arrays
Two-Dimensional Array:  (array যেখানে প্রত্যেকটা ভ্যালু আরেকটা array )    
Three-Dimensional Array: (array যেখানে প্রত্যেকটা ভ্যালু two-dimensional array) 
N-Dimensional Array:  (Arrays with more nested levels)


Two-Dimensional Array : Two-Dimensional Array হলো একটা multiple array , যেটা row এবং column মতো আচরণ করে। একটা উদাহরণ দেওয়া হল। 

```
$products = [   ["Laptop", 1200, 5],["Smartphone", 800, 10],["Tablet", 400, 7]   ];
```

               
এটা একটা Two-Dimensional Array . কারণ এখানে $products একটা main array ,এবং এর মধ্যে যে ভ্যালু গুলো assign  আছে, সেগুলো ও এক একটা array . 
এবার আসি এটা কিভাবে  row এবং column মতো আচরণ করে। এখানে main Array টা হচ্ছে row এবং এর ভিতর যে ভ্যালু হিসাবে array গুলো আছে সেগুলো হচ্ছে column . অর্থাঃ 
               
```               
$products = [   

["Laptop",        1200,                5],             =======> first row (0 index)
    ।                ।                  ।
    ।                ।                  ।
(1r  ,1c  )     (1r ,2c )       (1r ,3c )
(0 index)      (1 index)     (3 index)



["Smartphone",         800,          10],    =======> second  row (1 index)

    ।                    ।                  ।
    ।                    ।                  ।
(2r  ,1c  )         (2r ,2c )       (2r ,3c )

(0 index)           (1 index)     (3 index)


["Tablet",        400,             7]                 =======> third  row (2 index)

    ।                ।               ।
    ।                ।               ।
(3r  ,1c  )     (3r ,2c )       (3r ,3c )
(0 index)      (1 index)     (3 index)

];
```

Three-Dimensional (3D) Array : Three-Dimensional  Array হয় এক ধরণের মাল্টিপল array .যেখানে main array এর প্রতি টা ভ্যালু 
two-dimensional array . নিচে Associative Arrays উদাহরণ দেয়া হল বুঝার সুবিধার জন্য। 

```
    $school = [
    
        "Class 1" => [
            ["Rasel", "A+"],
            ["Rahim", "B"]
    
        ],
    
        "Class 2" => [
            ["Karim", "A"],
            ["Jamal", "C"]
    
        ]
    ];

    নিচে আরেকটা উধাহরন দেওয়া হল 

    $school = [
    
    [
        ["Rasel", "A+"],
        ["Rahim", "B"]

    ],

    [
        ["Karim", "A"],
        ["Jamal", "C"]

    ]
];
```

এখানে $school একটা main array যেখানে ভ্যালু হিসাবে আছে two dimension array .

N-Dimensional Array :  N-Dimensional array মানে হল  main array এর ভিতর ভ্যালু হিসাবে (সাধারণত array ভ্যালুগুলো  index হিসাবে থাকে যেমন ০,১। ওই ০ index যত তত array ) যত তত array .একটা উদাহরণ নিচে দেয়া হল। 

```
    $universe = [
    [
        [
            ["Life Exists", "Oxygen Available"]
        ]
    ],

[
    [
        ["Life not Exists", "Oxygen not Available"]
    ]
    ]
]
```
Behind the seen in Array (how its work): 
যখন তুমি একটা অ্যারে তৈরি করো, PHP এটি RAM-এ সংরক্ষণ করে। প্রতিটি মান (value) একটি নির্দিষ্ট মেমরি ঠিকানায় (Memory Address) থাকে, যা CPU দ্রুত এক্সেস করতে পারে।

কীভাবে PHP অ্যারে RAM-এ কাজ করে?

1️⃣ তুমি যখন $array = ["Apple", "Banana", "Mango"]; লিখো, PHP এটি RAM-এ সংরক্ষণ করে।
2️⃣ প্রতিটি মানের জন্য একটি Memory Address থাকে, যেমন:

```
Index	Value	Memory Address (RAM)
0	Apple	        0x100
1	Banana	        0x104
2	Mango	        0x108
3️⃣ যখন তুমি echo $array[1]; লিখো, PHP RAM থেকে 0x104 অ্যাড্রেস থেকে "Banana" নিয়ে আসে।
```

## superglobal variables
        
1.$_GET – URL থেকে ডাটা নেওয়া
$_GET ব্যবহার করে আমরা URL-এর মাধ্যমে পাঠানো ডাটা সংগ্রহ করতে পারি।
উদাহরণ : ধরো, তোমার URL হলো – https://example.com?name=Rasel&age=25
এখন, PHP-তে এই ডাটা $_GET দিয়ে পাওয়া যাবে –

```
<?php
echo "নাম: " . $_GET['name'] . "<br>";
echo "বয়স: " . $_GET['age'];
?>
```
ব্যবহার: যখন আমরা লিংকের মাধ্যমে ডাটা পাঠাতে চাই, তখন $_GET ব্যবহার করি।        

2.ব্যবহার: $_POST সাধারণত সিকিউর ডাটা পাঠানোর জন্য ব্যবহৃত হয়, কারণ এটা URL-এ দেখা যায় না।
উদাহরণ: ধরো, আমাদের একটা লগইন ফর্ম আছে –    

```
<form action="process.php" method="POST">
    ইউজারনেম: <input type="text" name="username"><br>
    পাসওয়ার্ড: <input type="password" name="password"><br>
    <input type="submit" value="লগইন">
</form>
```

এখন যে ফাইল আমরা ডাটা দেখাবো সেখানে নিচের কোড লিখলে 

```
<?php
echo "ইউজারনেম: " . $_POST['username'] . "<br>";
echo "পাসওয়ার্ড: " . $_POST['password'];
?>
```

আউটপুট (যদি ইউজার 'Rasel' এবং '1234' দেয়)

3.$_REQUEST – GET ও POST দুইটাই গ্রহণ করে     
উদাহরণ:  

```
<?php
echo "নাম: " . $_REQUEST['name'];
?>
```

ব্যবহার: যখন আমরা জানি না যে ডাটা $_GET নাকি $_POST দিয়ে আসবে, তখন $_REQUEST ব্যবহার করা হয়।


4.$_FILES – ফাইল আপলোড করার ক্ষেত্রে বেবহার হয় 

5.$_SERVER – ব্যবহার করে  সার্ভার সংক্রান্ত তথ্য পাওয়া যায়।  
উদাহরণ : 

```
<?php
echo "তোমার IP: " . $_SERVER['REMOTE_ADDR'] . "<br>";
echo "তোমার ব্রাউজার: " . $_SERVER['HTTP_USER_AGENT'] . "<br>";
?>
```

তোমার IP: 192.168.1.1  
তোমার ব্রাউজার: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
        
6.$_ENV – সার্ভারের এনভায়রনমেন্ট তথ্য পাওয়া
উদাহরণ : 

```
<?php
echo "সার্ভার নাম: " . $_ENV['HOSTNAME'];
?>
```

ব্যবহার: যখন আমরা সার্ভারের তথ্য সংগ্রহ করতে চাই।


7.$_GLOBALS –  ব্যবহার করা হয় , সব ধরণের ভেরিয়াবলে এক্সেস করার জন্য 
উদাহরণ : 

```
<?php
$name = "Rasel";
function myFunction() {
    echo "নাম: " . $GLOBALS['name'];
}
myFunction();
?>
```    
ব্যবহার: যখন আমরা ফাংশনের বাইরে থাকা ভেরিয়েবল ফাংশনের ভিতরে ব্যবহার করতে চাই।    

8.$_SESSION এবং $_COOKIE একই জিনিস নয়, বরং এদের মধ্যে কিছু পার্থক্য আছে।

### $_SESSION 

1.সার্ভার সাইডে সংরক্ষণ হয়। 
2.যতক্ষণ ব্রাউজার বন্ধ না হয় বা ম্যানুয়ালি session_destroy() না করা হয় ,তথক্ষণ পযন্ত ডাটা থাকে?
3.বেশি নিরাপদ, কারণ ডাটা সার্ভারে থাকে।  $_SESSION এর ডাটা সার্ভারের টেম্পোরারি মেমোরিতে (RAM) বা ফাইল সিস্টেমে সংরক্ষণ হয়।
4.সাধারণত /tmp/sess_abc123 এরকম ফোল্ডারে ফাইল তৈরি হয়।
5.$_SESSION ব্যবহার করে সার্ভারে থাকা ডাটা অ্যাক্সেস করা যায়
6.$_SESSION ব্যবহার করুন যখন ডাটা সিকিউর রাখতে চান, যেমন লগইন ইনফরমেশন।

### $_COOKIE

১. ইউজারের ব্রাউজারে সংরক্ষণ হয়
২.কুকি মেয়াদ শেষ হওয়া পর্যন্ত ব্রাউজারে থাকে (একদিন, এক সপ্তাহ বা এক মাস পর্যন্ত হতে পারে) . এটা সেট করা যায় 
৩.কম নিরাপদ, কারণ ইউজার কুকি পরিবর্তন করতে পারে
৪.$_COOKIE ব্যবহার করে ব্রাউজারে থাকা ডাটা পাওয়া যায়
৫.কুকির জন্য সাধারণত 4 KB সীমাবদ্ধতা থাকে

৬.$_COOKIE এর ডাটা ইউজারের ব্রাউজারে (Client Side) সংরক্ষণ হয়।
৭. Chrome/Firefox ব্রাউজারের Application → Cookies সেকশনে কুকি দেখা যায়।


## PHP Advance

PHP include এবং require : PHP-তে include এবং require দুটি ফাংশন ব্যবহার করা হয় একটি ফাইলকে অন্য ফাইলে অন্তর্ভুক্ত করার জন্য। নিচে উদাহরণ দেয়া হল 
উদাহরণ :  ধরা যাক আমার কাছে দুইটা  ফাইল আছে  একটা হল main.php এবং ওপরটা হল header.php এখন main.php এর ভিতর  যদি header.php অন্তর্ভুক্ত করতে হয় তাহলে দুই ভাবে করা যায়। 
একটা inclue ব্যবহার করে আরেকটা required ব্যবহার করে 

```
<?php
include "header.php";  
require "header.php";
?>
```

### include 
include ব্যবহার করলে যদি ফাইলটি না পাওয়া যায়, তাহলে PHP একটি Warning (E_WARNING) দেখাবে,
কিন্তু স্ক্রিপ্ট বা বাকি code  চলতে থাকবে।

উদাহরণ 

```
<?php
echo "Before including the file.<br>";
include "header.php";  // যদি `header.php` না পাওয়া যায়, তবুও কোড চলবে
echo "After including the file.<br>";
?>
```

এবার  যদি  header.php ফাইল টা না পাওয়া যায় ,তাহলে একটা warning show করবে এবং বাকি স্ক্রিপ্ট টুকু run করবে 
output অনেকটা এরকম দেখাবে 

Before including the file.
Warning: include(header.php): Failed to open stream: No such file or directory in index.php on line 3
After including the file.


### require 
require ব্যবহার করলে যদি ফাইলটি না পাওয়া যায়, তাহলে PHP Fatal Error (E_ERROR) দেখাবে এবং পুরো স্ক্রিপ্ট থেমে যাবে। বাকি code টুক 
আর run হবে না 
উদাহরণ :
require ব্যবহার করলে যদি ফাইলটি না পাওয়া যায়, তাহলে PHP Fatal Error (E_ERROR) দেখাবে এবং পুরো স্ক্রিপ্ট থেমে যাবে।   
                
### include_once এবং require_once : 

কখনো কখনো একই ফাইল একাধিকবার ইনক্লুড হয়ে যেতে পারে, যা সমস্যা তৈরি করতে পারে।
এটি প্রতিরোধ করতে include_once এবং require_once ব্যবহার করা হয়, যা একই ফাইল শুধুমাত্র একবার লোড করবে।   
                
উদাহরণ :

```
<?php
include "config.php"; 
include "config.php";
?>
```

📌 এখানে config.php দুইবার include করা হয়েছে, যার ফলে:
1️⃣ যদি config.php-তে কোনো ফাংশন বা ক্লাস ডিফাইন করা থাকে, তাহলে "function/class already declared" এরর আসতে পারে।
2️⃣ একই সেটিংস বা ভেরিয়েবল দুইবার লোড হলে কনফ্লিক্ট তৈরি হতে পারে।

সে ক্ষেত্রে include_once  ব্যবহার করলে এটি দ্বিতীয়বার লোড হবে না। অথাৎ "config.php ফাইল টা একবারই load হবে। reuired এর ক্ষেত্রে ও 
একই নিয়ম 

```
<?php
include_once "config.php"; 
include_once "config.php";
?>
```

## PHP File Upload 
                
    
PHP File Upload করতে কিছু বেসিক রুল follw করতে হয় এগুলো নিচে দেয়া হল। 

১। প্রথমে একটা ফর্ম লাগবে 
২। এর input type হবে file .
৩। আরেকটি হল enctype="multipart/form-data" এটি ফাইল ডাটা সঠিক ভাবে পাঠানোর জন্য দরকার     
main topice আলোচনা করার আগে কিছু জিনিস clear হওয়ার দরকার 

### 📌 enctype="multipart/form-data" মানে কী?

enctype="multipart/form-data" হল একটি HTML form attribute, এটা ব্যবহার করা হয়, যখন ফর্মের মাধ্যমে ফাইল আপলোড করতে হয়।
        
### 📌 enctype কী?
একটি ফর্মে আমরা অনেক রকমের ডাটা পাঠাতে পারি, যেমন:সাধারণ টেক্সট (Text) – নাম, ইমেইল, পাসওয়ার্ড ইত্যাদি ফাইল (File) – ছবি, পিডিএফ, ওয়ার্ড ডকুমেন্ট ইত্যাদি
এখন, ব্রাউজার যখন এই ডাটাগুলো সার্ভারে পাঠায়, তখন সেটাকে এক বিশেষভাবে এনকোড (Encode) করে পাঠাতে হয়।
এটাই Encoding Type (enctype)!

### 📌 আরো  enctype type আছে ,সেগুলো হল 
        
Encoding Type	                                            ব্যবহার
application/x-www-form-urlencoded	                        (ডিফল্ট) সাধারণ text data পাঠানোর জন্য
multipart/form-data	                                        (ফাইল আপলোড করার জন্য)
text/plain	                                                 সাধারণ text data পাঠানোর জন্য (কম ব্যবহার হয়)

নিচে details আলোচনা করা হল :

### ✅ ১. application/x-www-form-urlencoded (ডিফল্ট) (যখন get method use করা হয়) .

যখন কোন সাধারণ টেক্সট ডাটা (যেমন: নাম, ইমেইল, পাসওয়ার্ড) পাঠানো হয় , তখন ব্রাউজার এই enctype ব্যবহার করে।
এটি ফর্মের ডাটাকে, URL ফরম্যাটে এনকোড করে পাঠায়।

উদাহরণ:

যদি ফর্মে নাম: Rasel এবং ইমেইল: rasel@gmail.com দেয়া হয় , তখন ব্রাউজার এটিকে  এভাবে পাঠাবে—

```
name=Rasel&email=rasel%40gmail.com
```

যখন post method use করা হয় ,তখন ডাটা এমন ভাবে যায়। যেখানে ফর্মটা দেখতে এরকম 

```
<form action="process.php" method="POST">
    Name: <input type="text" name="name"><br>
    Email: <input type="email" name="email"><br>
    <input type="submit" value="Submit">
</form>
```

ফর্ম সাবমিট করা হয় , তখন ব্রাউজার এই ডাটা সার্ভারে পাঠায় এইভাবে 
```
POST /process.php HTTP/1.1
Host: example.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 27
name=Rasel&email=rasel@gmail.com
```

📌 এখানে:
✅ POST /process.php HTTP/1.1 → ফর্মটি process.php-তে পাঠানো হচ্ছে।
✅ Content-Type: application/x-www-form-urlencoded → ডাটা এনকোড করা হয়েছে।
✅ name=Rasel&email=rasel@gmail.com → ডাটা Request Body-তে আছে, URL-এ না!



### ✅ ২. multipart/form-data (ফাইল পাঠানোর জন্য)

যখন তুমি ফাইল পাঠাতে চাও, তখন enctype="multipart/form-data" ব্যবহার করতে হবে।
এটি প্রত্যেকটি ইনপুট ফিল্ডের ডাটাকে আলাদা "part" আকারে পাঠায়, যাতে ফাইলের বাইনারি ডাটা (binary data) ঠিকমতো পাঠানো যায়।

👉 যদি enctype="multipart/form-data" ব্যবহার করা হয়, তাহলে ফর্মের ডাটা এমনভাবে যাবে:

```
------WebKitFormBoundaryxYz
Content-Disposition: form-data; name="name"

Rasel
------WebKitFormBoundaryxYz
Content-Disposition: form-data; name="email"

rasel@gmail.com
------WebKitFormBoundaryxYz
Content-Disposition: form-data; name="myfile"; filename="profile.jpg"
Content-Type: image/jpeg
(binary data)
```

[এখানে ফাইলটি বাইনারি ডাটা আকারে পাঠানো হয়েছে, যা সাধারণ application/x-www-form-urlencoded দিয়ে সম্ভব নয়।]

           
### ✅ ৩. text/plain (কম ব্যবহৃত হয়)
এটি সাধারণ প্লেইন টেক্সট হিসেবে ফর্মের ডাটা পাঠায়।
এতে স্পেশাল ক্যারেক্টারগুলোকে  এনকোড করা হয় না।
উদাহরণ:
যদি তুমি ফর্মে নাম: Rasel এবং ইমেইল: rasel@gmail.com দাও, তাহলে এটি এমনভাবে যাবে—

```
name=Rasel
email=rasel@gmail.com
```


### 📌 $_FILES কী ?
$_FILES একটি সুপারগ্লোবাল (Superglobal) অ্যারে, যা HTML ফর্ম থেকে আপলোড করা ফাইলের তথ্য সংগ্রহ করতে ব্যবহৃত হয়।
            
সহজভাবে বললে, যখন একজন ইউজার একটি ফাইল আপলোড করে, তখন $_FILES অ্যারেতে সেই ফাইলের নাম, সাইজ, টাইপ, টেম্পোরারি লোকেশন ইত্যাদি সংরক্ষিত থাকে।        
এবার আসি কিভাবে file php তে আপলোড করা হয়। 
প্রথমে HTML form তৈরি করতে হবে, যেখানে ইউজার ফাইল নির্বাচন করে আপলোড করতে পারবে।

```
<form action="upload.php" method="post" enctype="multipart/form-data">
    <input type="file" name="myfile">
    <button type="submit" name="submit">Upload</button>
</form>
```

```
<?php
if (isset($_POST['submit'])) {
$file = $_FILES['myfile']; // ফাইল ডাটা নেওয়া

// ফাইলের তথ্য সংগ্রহ করা
$fileName = $file['name'];      // ফাইলের নাম
$fileTmpName = $file['tmp_name']; // টেম্পোরারি লোকেশন
$fileSize = $file['size'];      // ফাইলের সাইজ
$fileError = $file['error'];    // কোন এরর আছে কিনা
$fileType = $file['type'];      // ফাইলের টাইপ

// আপলোড ফোল্ডার সেট করা
$uploadFolder = "uploads/";

// চেক করা যে, কোন এরর আছে কিনা
if ($fileError === 0) {
    // ফাইল সার্ভারে সংরক্ষণ করা
    move_uploaded_file($fileTmpName, $uploadFolder . $fileName);
    echo "✅ ফাইল সফলভাবে আপলোড হয়েছে!";
} else {
    echo "❌ ফাইল আপলোড করতে সমস্যা হয়েছে!";
}
}
?>
$file = $_FILES['myfile'];
```

✔️ $_FILES হলো সুপারগ্লোবাল ভেরিয়েবল (এরে ) যা ফর্মের ফাইল ইনপুট (<input type="file" name="myfile">) থেকে ফাইল এর  ডাটা নিয়ে আসে, 
সহজ ভাষায়  যে ফাইল টা আমি choose করেছি আপলোড করার জন্য,  সে ফাইল এর ডাটা (সব ইনফরমেশন)  আমি এই _FILES সুপারগ্লোবাল ভেরিয়েবল (এরে ) এর মাধ্যমে পাই। 
এটি ফাইলের সব ইনফরমেশন একটি অ্যারে আকারে দেয়।

✔️ $file ভেরিয়েবলে ফাইলের সব তথ্য রাখা হলো।     
    
    
যেহেতু ফাইল এর সব ইনফরমেশন এখন $file মধ্যে আছে ,এবং এই ইনফরমেশন গুলো array name  আকারে আছে। যেমন : name ,tmp_name, ইত্যাদি 

1.$file['name'] → ফাইলের অরিজিনাল নাম পাওয়া যাচ্ছে (যেমন: image.jpg)
2.$file['tmp_name'] → ফাইল আপলোড হওয়ার পর, সেটি সার্ভারের টেম্পোরারি লোকেশনে রাখা হয় (এটি সার্ভারের /tmp/ ফোল্ডারে 
অস্থায়ীভাবে সংরক্ষিত থাকে)। যেটা আপলোড ফোল্ডারে যাওয়ার জন্য রেডি থাকে। এবং এটা আপলোড না করলে এটি কিছুক্ষন পর এমনি  রিমুভ হইয়া যায়  
3.$file['size'] → ফাইলের সাইজ (বাইটে)
4.$file['error'] → চেক করা হচ্ছে কোনো এরর হয়েছে কিনা
5.$file['type'] → ফাইলের টাইপ (যেমন: image/jpeg, image/png)

move_uploaded_file() ফাংশন দিয়ে ফাইল uploads/ ফোল্ডারে রাখা হবে।

```
move_uploaded_file($fileTmpName, $uploadFolder . $fileName);
```
অর্থাৎ টেম্পোরারি লোকেশন থেকে ফাইল টা আপলোড ফোল্ডার এ অর্থাৎ যে ফোল্ডারে আমি ফাইল টা রাখতে চাই , এবং ফাইনালি কি নাম রাখতে চাই ওই নামটা concate করে দেয়া 


## Session and Cookies
ধরো, তুমি একটা পার্কে গেছো। এখন তুমি দুইভাবে প্রবেশ করতে পারো: (একটা Session আর একটা Cookies এর লজিক নিয়ে )

### Session:
1.পার্কে ঢোকার সময় আমাকে একটা প্রবেশ টিকিট (ID) দেওয়া হলো, যা পার্কের মালিকের কাছে সংরক্ষিত  আছে ।
2.যতক্ষণ আমি পার্কের ভিতরে থাকবো , ততক্ষণ আমি পার্কে ঘুরার এক্সেস পাবো। কারণ আমার টিকেটটি পার্কের মালিকের কাছে আছে। 
3.কিন্তু যখন আমি  পার্ক থেকে বের হয়ে যাব , তখন আমার টিকেটটি মালিক ফেলে দিবে। ফলে আমাকে আবার পার্কে ঢুকতে হলে আমাকে 
আবার টিকেট নিতে হবে। 

### PHP Session (সেশন)
Session সার্ভারে তথ্য সংরক্ষন করে রাখে , ইউজার যখন ওয়েবসাইটে ঢোকে তখন তৈরি হয় 
(অর্থাৎ যেখানে আমি session টা start করতেছি। উদাহরণ স্বরুপ বলা যেতে পারে ,ধরুন আমি চাচ্ছি যে ইউজার যখন লগইন করবে তখন তার user_name session এ  স্টোর করবো ,সে ক্ষেত্রে আমাকে লগইন পেজ session টা স্টার্ট করতে হবে।  ), 
এবং ব্রাউজার বন্ধ করলে মুছে যায়।

### কোথায় ব্যবহার করবো?
ইউজার লগইন করলে তার তথ্য রাখতে (যেমন: ইউজারের নাম, ইমেইল ইত্যাদি)
ওয়েবসাইটে কেনাকাটা করলে (Shopping Cart)
Session ব্যবহার করার জন্য টা session_start() লিখতে হবে।    

📌 PHP Session সার্ভারের কোথায় সংরক্ষণ করা হয়?
✔️ PHP ডিফল্টভাবে সেশন ডাটা, সার্ভারের /tmp ফোল্ডারে .sess_xxx ফাইল আকারে সংরক্ষণ করে রাখে ।
✔️ session_save_path() ব্যবহার করে সেশন ফাইলের অবস্থান চেক করা যায়। অর্থাৎ Session ফাইল টা কোথায় আছে সেটা জানা যায়। 
✔️ php.ini বা session_save_path() ব্যবহার করে সেশন লোকেশন পরিবর্তন করা যায়।
✔️ সেশন ডাটাবেজেও সংরক্ষণ করা সম্ভব। 🚀








### Cookies:
1.এবার ধরো, পার্কের ঢুকার সময় আমার হাথে  আমাকে একটা ছোট স্টিকার (Token) দেওয়া হলো, যেখানে আমার নাম লেখা আছে। এবং এর একটা এক্সেস টাইম দেয়া আছে। 
2.এখন আমি ওই সময় এর মধ্যে যতবার ইচ্ছা পার্কে ঢুকতে পারবো এবং বের হতে পারবো ,যতক্ষণ না আমার এক্সেস টাইম শেষ হচ্ছে। যেহেতু আমার হাতে স্টিকার আছে সেহেতু পার্কের মালিক ও আমাকে চিনবে। 

### PHP Cookies (কুকি)
Cookies ব্রাউজারে তথ্য সংরক্ষন করে রাখে , যা নির্দিষ্ট সময় পর্যন্ত থেকে যায়। এক কোথায় বলতে গেলে এটি user এর ছোট ছোট Activiti সংরক্ষন করে রাখে, যেটা তার কাজ টাকে সহজ করে দেয় নিচে এর কিছু উদাহরণ দেয়া হল। 
কোথায় ব্যবহার করবো?
1."Remember Me" অপশন তৈরি করতে, যাতে ইউজার পরে লগইন করতে না হয়
2.Language change  এর ক্ষেত্রে এটি ব্যবহার করা হয়। উদাহরণ স্বরূপ আমি একটা ওয়েবসাইটে ঢুকলাম যেখানে দুই টা language  আছে ইংলিশ  এবং বাংলা ,আমি বাংলা সিলেক্ট করলাম। এখন পরেরবার যখন আমি এই  ওয়েবসাইটে ঢুকব, তখন বাংলা language  টাই দেখাবে। 
Cookies সেট করার জন্য setcookie() ফাংশন ব্যবহার করতে হবে।


## PHP Filter
### PHP Filter 
PHP Filter কাজ হল ইনপুট data চেক করা। যাতে ইউজার ভুল বা খারাপ ডাটা না পাঠাতে পারে। নিচে এর কিছু উদাহরণ দেয়া হল। 

Filter	                                                                কাজ
FILTER_VALIDATE_EMAIL	                                        ইমেইল ঠিক আছে কিনা
FILTER_VALIDATE_INT	                                            সংখ্যা (integer) কিনা
FILTER_SANITIZE_STRING	                                        অপ্রয়োজনীয় জিনিস বাদ দেওয়া
FILTER_VALIDATE_URL                                             URL ঠিক আছে কিনা    


## Call back Functionr

### Callback Function মানে কী?
একটা function-এর ভিতরে যখন অন্য একটা function কে "parameter" হিসেবে পাঠানো হয় — এবং parameter হিসাবে পাঠানো ওই ফাঙ্কশন টাকে call করা হয় তখন 
তাকে Callback Function বলে। 
সহজ ভাবে বলতে গেলে function এর parameter হিসাবে যখন function pass করা হয় এবং পরে ওই pass করা function টাকে call করা হয় তখন তাকে Callback Function বলে। 

নিচে উদাহরণ দেয়া হল 

```
function greet($name) {
    echo "👋 Hello, $name!<br>";
}

function processUser($callback) {
    $users = ["Rasel", "Sumi", "Nayeem"];

    foreach ($users as $user) {
        // এখানে callback ফাংশনকে কল করা হচ্ছে
        $callback($user);
    }
}
```
processUser("greet"); // "greet" ফাংশন কে callback হিসেবে পাঠানো হলো

এখানে প্রথমে processUser function টা call করা হয়েছে। এবং perameter হিসাবে greet pass করা হয়েছে। 
processUser function এর ভিতর $users নামে একটা array আছে। এরপর ওই array টাকে foreach করা হয়েছে। যাতে array এর ভিতর ভ্যালু গুলো সিঙ্গেল ভ্যালু হিসাবে পাওয়া যায়। 
এখন এখানে   callback ফাংশনকে কল করা হচ্ছে  $callback($user); এর মানে হল এখানে greet($user) অর্থাঃ greet function টাকে call করা হয়েছে। 
[কারণ এখানে $callback perameter হিসাবে greet function টাকে pass করা হয়েছে  ] আরো সহজ ভাবে বলতে গেলে 
processUser("greet");
$callback = greet 
এখানে $callback এর ভ্যালু হচ্ছে greet . নরমাল function যেভাবে perameter pass করে আরকি।   

## OOP

### OOP 
Object-Oriented Programming (OOP) হচ্ছে এমন একটা প্রোগ্রামিং স্টাইল যেখানে আমরা সব কিছু object হিসেবে দেখি।
সহজ ভাবে যেখানে আমরা class আর object দিয়ে কোড লিখি    

### Class 
Class হলো একটা নকশা (blueprint) — যেখানে আমরা বলে দিই একটা জিনিস কেমন হবে, তার কি কি গুণ (property) থাকবে, আর সে কী কী কাজ (method) করতে পারবে। ধরা যাক আমি একটা গাড়ির বানানোর  নকশা তৈরী করবো ,সেখানে গাড়ির color ,brand ইত্যাদি বিষয় থাকবে। 

```
class Car {
    public $color;
    public $brand;

    public function drive() {
        echo "🚗 গাড়ি চলছে...";
    }
}
```
               
এখানে Car হল class বা নকশা। যেখানে color এবং brand দুইটা প্রপার্টি আছে। এবং একটা মেথড আছে।  এই হল class এর স্বভাব।   
           
### Object 
Object হলো class থেকে বানানো আসল জিনিস [ওই নকশা থেকে বানানো আসল জিনিষটা ] — মানে, সেই নকশা থেকে বানানো গাড়িটা ।

```
$car1 = new Car();
$car1->color = "লাল";
$car1->brand = "Toyota";
$car1->drive
```
               
এখানে $car1 হচ্ছে object .যেটা ওই নকশার বা class  আসল রূপ দিয়েছে যে ,গাড়িটার color হবে লাল এবং ব্র্যান্ড হবে Toyota .    
[এক কথায় বলতে গেলে class হল একটা নকশা , এবং নকশার উপর ভিত্তি করে আসল যে রূপ দেয়া হয় তা হল object]   
        

### Constructor 
Constructor হলো একটা Special Function (বিশেষ ফাংশন) এটাকে আবার magic function ও বলা হয়। যখন কোনো class এর 
object তৈরী করা হয় ,তখন এটি automatic ভাবে নিজে নিজে call হয়। এটাকে অন্য function এর মত call করার দরকার পরে না।   
এটা লিখা হয়  ( __construct ) এই ভাবে |   
         
### Destructor 
Destructor হলো একটা Special Function (বিশেষ ফাংশন) এটাকেও  magic function বলা হয়। কোন class যখন object তৈরি করি তখন Destructor function টা অটোমেটিক call হয়,Constructor এর মত। 
পার্থক্য হল Constructor সবার প্রথমে call হয় আর Destructor সবার শেষে call হয়। এটা লিখা হয়  ( __destruct ) এই ভাবে। 

### Access Modifier
Access Modifier : Access Modifier একটি ক্লাস এর প্রপার্টি এবং মেথড কে কত টুকু access করতে পারবে সেটা নির্ধারণ করে। 
তিন ধরণের Access Modifier আছে। নিচে আলোচনা করা হল। 

### Public 
কোন property বা মেথড এর আগে public থাকলে এটা সব জায়গা থেকে access করা যাবে (class এর ভিতর, class এর বাইরে, 
এমনকি অন্য class থেকেও)। 
নিচে আলোচনা করা হল। 

class এর ভিতর :
ক্লাস এর ভিতর যে মেথড বা প্রপার্টি আছে , ওই মেথড বা প্রপার্টি কে যদি ওই ক্লাস এর ভিতরের অন্য কোনো প্রপার্টি বা মেথড এক্সেস করে তখন তাকে ক্লাস এর ভিতর বলে 

উদাহরণ  : 

```
class Car {
public $brand = "Toyota";

public function showBrand() {
    // এটা class এর ভিতর থেকে access করছে $brand
    echo "Brand is: " . $this->brand;
}
}
```


class এর বাইরে :
class এর বাইরে বলতে বুঝায় , object বানিয়ে class এর property/method use করা       
                            
উদাহরণ :   

```
$car1 = new Car();        // class এর বাইরে object বানানো
echo $car1->brand;        // বাইরে থেকে public property access করা
$car1->showBrand();         // বাইরে থেকে public method access করা
```

অন্য class :
কোন একটা  class থেকে অন্য একটা  class এর public method/property access করা যায়। 

উদাহরণ  :

```
class A {
    public $msg = "I am from class A";
}

class B {
    public function showMessage() {
        $obj = new A();
        echo $obj->msg; // ✅ public বলে access করা যাচ্ছে
    }
}

$b = new B();
$b->showMessage(); // Output: I am from class A    
```

### protected 
protected property বা method কে সরাসরি object  তৈরী করে  access করা যায় না। এটা কে কেবল নিজ class এর ভিতর এবং child class থেকে access করা যায়। 

নিজ class থেকে access : 

```
class MyClass {
    protected $message = "I am protected!";

    public function showMessage() {
        // নিজের class এর ভিতর থেকে protected property access
        echo $this->message;
    }
}

$obj = new MyClass();
$obj->showMessage(); // ✅ কাজ করবে     
// echo $obj->message; // ❌ কাজ করবে না (কারণ এটিকে সরাসরি object তৈরী করে access করা হচ্ছে )   
```



child class থেকে access :

```
<?php

class ParentClass {
    protected function sayHello() {
        echo "👋 Hello from ParentClass!<br>";
    }
}

class ChildClass extends ParentClass {
    public function greet() {
        // এখানে protected method কে access করা হয়েছে
        $this->sayHello();
    }
}

$obj = new ChildClass();
$obj->greet(); // ✅ এখানে greet() method এর মাধ্যমে sayHello() কে access করা হলো


// $obj->sayHello(); [❌ এই লাইন Error দিবে, কারণ protected method সরাসরি access করা যাবে না]
```

### private 
private property বা method কে সরাসরি object  তৈরী করে  access করা যায় না এবং কি  child class থেকে access করা যায় না ।  
এটা কে কেবল নিজ class এর ভিতর থেকে access করা যায়।     

```                           
<?php
class SecretClass {
    private function whisper() {
        echo "🤫 এটা একান্তই গোপন কথা!";
    }

    public function reveal() {
        // নিজের ভেতরের private method access করা হচ্ছে
        $this->whisper();
    }
}

$obj = new SecretClass();
$obj->reveal(); [এটা ঠিক থাকে ভাবে কাজ করবে কারণ একে class ভিতর থেকে call করা হয়েছে ]


// $obj->whisper(); [// ❌ নিচের লাইন Error দিবে কারণ একে class বাহির থেকে call করা হয়েছে। ]
```

এক কথায় বলতে গেলে 

public	           সকল জায়গা থেকে ✅ (বাইরেও)
protected	       subclass এবং class-এর ভিতরে ✅
private	        শুধু নিজের class-এর ভিতরে ✅  


## Inheritance 
Inheritance মানে হল উত্তরাধিকার। একটু অন্য ভাবে বলতে গেলে একজন সন্তানের যেমন নিজের কিছু ব্যক্তিগত সম্পদ থাকে, 
যেগুলো সে নিজে অর্জন করছে । আবার উত্তরাধিকার সূত্রে সে তার পিতার থেকেও পিতার সম্পতি পায়। সে চাইলেই সে নিজের এবং পিতার 
সম্পত্তি ও access করতে পারে। Inheritance টাও ঠিক এরকমই যেখানে দুটি ক্লাস থাকে একটি হল parent class আরেকটা হল child class । 
যেখানে child class টা parent class এর property এবং method access করতে পারে, সাথে নিজের  property এবং method ও access করতে পারে। 

### কেন ব্যবহার করা হয়?
এটি প্রথমত ব্যবহার করা হয় যাতে একই কোড বার বার না লিখতে হয়। ধরা যাক আমার অনেক গুলো ক্লাস লাগবে কাজের জন্য। এবং প্রত্যেকটা ক্লাস কিছু কমন প্রপার্টি এবং মেথড রয়েছে এখন এই প্রপার্টি এবং মেথড গুলো যদি আমি প্রতিটা ক্লাস এ লিখি তাহলে কি হচ্ছে একই টিপের এর কোড বার বার লিখা হচ্ছে ফলে কোডের সুন্দর্য নষ্ট হচ্ছে সাথে সাথে কোড duplication হচ্ছে ,তাই এটা দূর করার জন্য Inheritance বেবহার করা হয়। 

উদাহরণ 

```
// প্যারেন্ট ক্লাস
class Animal {
    public function sound() {
        echo "Some generic sound";
    }
}

// চাইল্ড ক্লাস
class Dog extends Animal {
    public function bark() {
        echo "🐶 Dog says: Woof!";
    }
}

$dog = new Dog();
$dog->sound(); // প্যারেন্ট ক্লাসের মেথড ✅
$dog->bark();  // নিজের মেথড ✅
```

মনে রাখো:

বিষয়	                       ব্যাখ্যা
extends	                        keyword যেটা দিয়ে Inheritance হয়
Parent Class	                যেটা থেকে গুণ নেয়া হয়
Child Class	                    যেটা গুণ পায়
Reusability	                     Inheritance-এর মূল সুবিধা


## Polymorphism 
Polymorphism হল OOP-এর একটি ধারণা, যেখানে একই নামের একটি মেথড (function) বিভিন্ন class-এ ভিন্নভাবে কাজ করে, 
অর্থাৎ প্রতিটি object তার নিজস্বভাবে সেই মেথড বাস্তবায়ন (implement) করে।
একই মেথড — ভিন্ন ভিন্ন আচরণ = Polymorphism . override করাই Polymorphism এর মূল চালিকা শক্তি।

উদাহরণ :

```
class Animal {
    public function makeSound() {
        echo "Some generic sound";
    }
}

class Dog extends Animal {
    public function makeSound() {
        echo "Woof! 🐶";
    }
}

class Cat extends Animal {
    public function makeSound() {
        echo "Meow! 🐱";
    }
}

// এই ফাংশনটা জানে না আসলে কোন animal আসবে
function playSound(Animal $animal) {
    $animal->makeSound(); // একি method, কিন্তু কাজ আলাদা
}

playSound(new Dog()); // Woof!
playSound(new Cat()); // Meow!
```

এখানে makeSound() মেথড সব ক্লাসেই একই নামে আছে,
কিন্তু প্রতিটা অবজেক্ট আলাদা রকম সাউন্ড করছে – এটিই Polymorphism 🎭



### Polymorphism কনসেপ্ট এর  ব্যবহার 

Inheritance-based Polymorphism

```
class Animal {
    public function makeSound() {
        echo "Some generic sound";
    }
}

class Dog extends Animal {
    public function makeSound() {
        echo "Woof! 🐶";
    }
}

class Cat extends Animal {
    public function makeSound() {
        echo "Meow! 🐱";
    }
}

// এই ফাংশনটা জানে না আসলে কোন animal আসবে
function playSound(Animal $animal) {
    $animal->makeSound(); // একি method, কিন্তু কাজ আলাদা
}

playSound(new Dog()); // Woof!
playSound(new Cat()); // Meow!


```

এখানে makeSound() মেথড সব ক্লাসেই একই নামে আছে,
কিন্তু প্রতিটা অবজেক্ট আলাদা রকম সাউন্ড করছে (আউটপুট দিতেছে) – এটিই Polymorphism 

Interface-based Polymorphism
একটা interface থাকে যেখানে কেবল method declaration থাকে (মানে কাজ কী হবে তা বলা থাকে না, শুধু method-এর নাম ও signature থাকে)।
এরপর এক বা একাধিক class সেই interface implement করে — এবং নিজেদের মতো করে সেই মেথডের কাজ define করে।
একি method name → ভিন্ন class → ভিন্ন আচরণ → এটাই Polymorphism।



```
interface Animal {
    public function makeSound(); // শুধু ঘোষনা
}

class Cat implements Animal {
    public function makeSound() {
        echo "Cat says: Meow! 🐱";
    }
}

class Dog implements Animal {
    public function makeSound() {
        echo "Dog says: Woof! 🐶";
    }
}

// Function accepts any object that implements Animal
function playSound(Animal $animal) {
    $animal->makeSound();
}

playSound(new Cat()); // Output: Cat says: Meow!
playSound(new Dog()); // Output: Dog says: Woof!
```


  
ব্যাখ্যা:
interface Animal → contract (চুক্তি): "makeSound" method must exist.
Cat এবং Dog → আলাদা class, কিন্তু দুইটিই Animal interface follow করে।
ফলে, playSound() ফাংশন বুঝেই না, আসলে কোন class আসবে — কিন্তু কাজ ঠিকই হয়।
Polymorphism কেবল Inheritance আর Interface-এর মাঝেই সীমাবদ্ধ না — তবে PHP-তে মূলত আমরা এই দুইটির মাধ্যমেই সবচেয়ে বেশি Polymorphism প্রয়োগ করি।


## Interface
Interface হলো এমন একটি কাঠামো (structure), যেখানে শুধু method-এর নাম define করা হয়, কিন্তু method-এর ভিতরে কী কাজ হবে — সেটা define করা হয় না। 
এবার এই Interface বা কাঠামো implement করে যে class গুলো বানানো হয় ,তারা ওই method গুলো ব্যবহার করে অর্থাৎ (method গুলোর ভিতরে কি হবে )। 
[interface এ সরাসরি object বানানো যায় না ]

উদাহরণ দিয়ে চিন্তা করো:
তুমি যদি একটা রোবট বানাও, তুমি আগে থেকে বলে দিতে পারো –
“এই রোবটকে কথা বলতে, হাঁটতে আর কাজ করতে পারতে হবে।”
কিন্তু রোবট কীভাবে হাঁটবে, কীভাবে বলবে — সেটা পরে ঠিক করবে।

example 

```
interface Animal {
    public function makeSound(); // শুধু method declured করা আছে। কোনো body নেই। 

}
```

Animal interface implements করে , dog class বানানো হয়েছে। এবং সে ওই interface এর method কে তার মত করে রূপ দিচ্ছে 

```
class Dog implements Animal {
    public function makeSound() {
        echo "Woof! 🐶";
    }
}
```

Animal interface implements করে , dog class বানানো হয়েছে। এবং সে ওই interface এর method কে তার মত করে রূপ দিচ্ছে 

```
class Cat implements Animal {
    public function makeSound() {
        echo "Meow! 🐱";
    }
}
```


Multiple Interface implement

```
interface Logger {
    public function log($msg);
}

interface Notifier {
    public function notify($msg);
}

class UserActivity implements Logger, Notifier {
    public function log($msg) {
        echo "Logging: $msg<br>";
    }

    public function notify($msg) {
        echo "Notifying: $msg<br>";
    }
}
```    


ব্যবহার:

```
function playSound(Animal $animal) {
    $animal->makeSound();
}

$dog = new Dog();
$cat = new Cat();

playSound($dog); // Woof!
playSound($cat); // Meow!
```

এখানে আরেকটা বিষয় আছে সেটা হল। তুমি যদি কোনো interface implements করে class বানাও ,তাহলে ওই implement এর যত গুলো method আছে ,
সেগুলো ওই class এ অব্যশই add করতে হবে। পাশাপাশি তুমি চাইলে বাড়তি method ও ওই class এ add করতে পারবে |   
             
কেন Interface ব্যবহার করি?
নিয়ম তৈরি করতে	
Multiple class-এর common behavior নিশ্চিত করতে	
Dependency Injection / Loose Coupling কোডে flexibility আসে, পরিবর্তন সহজ হয়
Polymorphism


Interface vs Class:

```
বিষয়	                Interface	                                        Class

কী define করে	        শুধুমাত্র method-এর নাম	                               method নাম + কাজ
properties থাকে?	    ❌ না	                                        ✅ হ্যাঁ
method body থাকে?	    ❌ না	                                        ✅ হ্যাঁ
implements / extends	implements দিয়ে implement করতে হয়	            extends দিয়ে inherit করতে হয়
```


## Abstract Class 
এটা একটা আধা-সম্পূর্ণ class — কিছু কাজ নিজে করে, কিছু future subclass দিয়ে করায়। একটু বুঝিয়ে বলতে গেলে। 
Abstract Class এ কিছু method আছে যেগুলো body পার্ট থাকে (যে কাজ গুলো সে নিজে করে )। আবার কিছু method আছে যেটা শুধু declured করা। 
এর কোনো বডি পার্ট নাই ( যেটা subclass দিয়া করায় ) । যেসব method শুধু define করা থাকে , তাকে abstract বলে, এর বডি পার্ট হয় না। [abstract class থেকে সরাসরি object তৈরি করা যায় না। abstract method গুলো child class কে অব্যশই ব্যবহার করতে হবে ]  
উদাহরণ :

```
abstract class Animal {
// এই method এর ভিতর এর কাজ গুলো সে নিজে করেছে। 
    public function eat() {
        echo "Eating food<br>";
    }

// এই method এর কাজ গুলো subclass দিয়া করাইছে। 
    abstract public function makeSound(); // শুধু define করা হলো
}


class Dog extends Animal {
    public function makeSound() {
        echo "Dog says: Woof! 🐶<br>";
    }
}

class Cat extends Animal {
    public function makeSound() {
        echo "Cat says: Meow! 🐱<br>";
    }
}


$dog = new Dog();
$dog->eat();          // Eating food
$dog->makeSound();    // Dog says: Woof!

$cat = new Cat();
$cat->eat();          // Eating food
$cat->makeSound();    // Cat says: Meow!
```



          
### কেন ব্যবহার করা হয় Abstract Class?

```
কারণ	                                                                 ব্যাখ্যা
✅ ১. Template বা structure তৈরি করতে	                                Child ক্লাসগুলো যেন ঠিক মতো একই গঠন (method) অনুসরণ করে
✅ ২. কিছু common behavior define করতে	                                যেমন eat() method সব Animal এর জন্য একই, তাই সেটি abstract class-এ একবারই define করবো
✅ ৩. Force করা child class গুলোকে specific method implement করতে	  যেমন makeSound() সব ক্লাসে আলাদা হবে, তাই child ক্লাসকে বাধ্য করবো implement করতে  
```  
          
          

### তুলনামূলক চার্ট (Interface vs Abstract Class):

```
বিষয়	                                           Interface	                                       Abstract Class
👉 কী	                                           সম্পূর্ণ design	                                      আধা design + কিছু কাজ
👉 object create করা যায়?	                       না ❌	                                              না ❌
👉 Constructor থাকে?	                           না ❌	                                              হ্যাঁ ✅
👉 Property/Variable define করা যায়?	           না ❌	                                              হ্যাঁ ✅
👉 Method implement করা যায়?	                   না ❌	                                              হ্যাঁ ✅
👉 Multiple implement?	                           হ্যাঁ ✅ (many interface)	                             না ❌ (একটিই class extend করা যায়)
👉 সব method override বাধ্যতামূলক?	                হ্যাঁ ✅	                                              না ❌ (শুধু abstract method-ই বাধ্যতামূলক)
👉 Access modifier (public/protected/private)     সব method public হয়	                               সব ধরনের modifier ব্যবহার করা যায়
👉 Use case	                                      Contract/Standard define	                            Common logic reuse + structure
```


## Traits 
Trait হলো PHP-র একটি special feature, যেটা ব্যবহার করা হয় code reuse (একই কোড বারবার লেখার ঝামেলা থেকে বাঁচতে)।
PHP-তে একটা class শুধু একটিই parent class extend করতে পারে (single inheritance)। এটা PHP একটা সীমাবদ্, আর এই সীমাবদ্ধ দূর করার জন্য Trait ব্যবহার করা হয়। 
কারণ একটা class একাধিক trait use করতে পারে। 

উদাহরণ : 

```
// Trait তৈরি করা
trait Printer {
    public function printData($data) {
        echo "Printing: $data<br>";
    }
}

// class এ trait ব্যবহার করা
class Invoice {
    use Printer;
}

class Report {
    use Printer;
}

$inv = new Invoice();
$inv->printData("Invoice #101");

$rep = new Report();
$rep->printData("Monthly Report");
```



single inheritance সীমাবদ্ধ কিভাবে Trait এর মাধ্যমে দূর হল :
আমরা জানি PHP single inheritance অর্থাৎ  PHP-তে একটা class শুধু একটিই parent class extend করতে পারে, multiple parent class 
extend করতে পারে না। 
একটা উদাহরণ দিয়া বুজানো হল 

```
Class Logger {
    public function log($msg) {
        echo "Log: $msg<br>";
    }
}

Class Printer {
    public function print($msg) {
        echo "Print: $msg<br>";
    }
}

class User extends Logger, Printer  {

}
```

এখানে দুইটা Class, Logger এবং Printer, User হচ্ছে একটা subclass যেটা  Logger এবং Printer কে extends করেছে। কিন্তু এইটা error দিবে 
কারণ একটা subclass একাধিক class কে extends করতে পারে না। PHP তে একটা subclass কেবল একটা parent class কে extends করতে 
পারে। 
এবার আসি Trait কিভাবে এই সীমাবদ্ধ দূর করলো। একটা উদাহরণ দিলে বুজতে ভালো হবে 

উদাহরণ 

```
trait Logger {
    public function log($msg) {
        echo "Log: $msg<br>";
    }
}

trait Notifier {
    public function notify($msg) {
        echo "Notify: $msg<br>";
    }
}

class User {
    use Logger, Notifier;
}

$user = new User
user->log('ok')
user->notify('ok')
```
এখানে Logger এবং Printer দুইটা trait . এবং User একটা class যে একাধিক trait use করতে পারতেছে, subclass যেভাবে parentClass extends করে। 


## Static Keyword 
আমরা জানি কোনো class এর method বা property access করতে হলে। ওই class এর object এর মাধ্যমে করতে হয়। কিন্তু 
কোন class এর method বা property তে Static Keyword use করলে তাকে object ছাড়াই,সরাসরি class দিয়া access করা যায়। 
নিচে একটা উদাহরণ দেয়া হল 

```
class MathHelper {
public static $pi = 3.1416;

public static function square($n) {
return $n * $n;
}
}

// Object ছাড়াই ব্যবহার:
echo MathHelper::$pi;             // Output: 3.1416
echo MathHelper::square(5);       // Output: 25
```

কেন ব্যবহার করবো?

```
দরকার	                                                                                  কারণ
✅ Common value রাখতে	                                                                 যেমন pi, VAT, siteName
✅ Utility functions (Helper function )	                                                 যেমন Helper::formatDate()
```

## Final Keyword 
সাধারণত php তে একটা subclass parent class কে extends করতে পারে এবং চাইলে  তার method কে override করতে পারে। 
এই কাজ টা যেন না করতে পারে এর জন্য Final Keyword বেবহার করা হয়। একটা উদাহরণ দেয়া হল। 

উদাহরণ ১: final class 

```
final class Bank {
public function withdraw() {
    echo "Withdraw successful";
}
}
// class SonaliBank extends Bank {}  // Final class extend করা যাবে না
```

উদাহরণ ২: final method

```
class Animal {
    final public function eat() {
        echo "Eating food";
    }
}

class Dog extends Animal {
    
    // public function eat() {}  // final method override করা যাবে না
}
```

কেন ব্যবহার করবো?

```
দরকার	                                                 কারণ
✅ Security	                                            কেউ subclass-এ ভুল করে override করে না
✅ Control	                                             Core method কেউ না পাল্টায়  
```
## Type Hinting 
PHP-তে Type Hinting মূলত function/method-এর parameter এবং return type-এর ক্ষেত্রেই ব্যবহৃত হয়। 
এর কাজ হল function/method-এর parameter এবং return type টা কি typer হবে ,অর্থাৎ [int ,string ,ইত্যাদি ]

### কোথায় কোথায় Type Hinting করা যায়?

```
কোথায়	                                                           কীভাবে	                                                                         উদাহরণ
1️⃣ Function Parameter	                                            টাইপ দিয়ে নির্দিষ্ট করা                                                               function add(int $a, int $b)
2️⃣ Function Return Type	                                        : type দিয়ে	                                                                      function getName(): string
3️⃣ Constructor Injection (OOP)                                     ক্লাস টাইপ hint	                                                                   __construct(Logger $logger)
4️⃣ Closure (anonymous function)	                                Arrow function বা normal	                                                      function (int $id): string
```

উদাহরণ:
Parameter Type Hinting : 

```
<!-- function এর perameter টা string হবে  -->
function greet(string $name) {
echo "Hello, $name!";
}
```

Return Type Hinting

```
<!-- এখানে রিটার্ন type টা intger হবে , যেটা :int  হিসাবে বলা আছে  -->
    function add(int $a, int $b): int {
    return $a + $b;
}
```

Object/Class টাইপ Hinting

```
class User {
    public function greet() {
        echo "Hi!";
    }
}

<!-- এখানে welcome function এর ভিতর perameter হিসাবে কেবল User এর অবজেক্ট ই pass করা যাবে। অন্য কিছু যাবে না   -->
function welcome(User $user) {
    $user->greet();
}

<!-- এটা error দিবে  -->
$animal = new Animal();  
welcome($animal);  

<!-- আবার কাজ করবে  -->
$animal = new User();  
welcome($animal);  
```




