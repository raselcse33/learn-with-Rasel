

<h1 align="center">Hi 👋, I'm Rasel Munshi</h1>
<h3 align="center">A Passionate Fullstack Developer from Bangladesh</h3>



# PHP Topics Start

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
function এর ভিতরের কোনো variable কে  Local Scope বলে. 
এর মানে কোনো ভ্যারিয়েবল function এর ভিতর declured করলে কেবলমাত্র ফাঙ্কশন এর ভিতরই access করা যাবে। 
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

## Exception Handling 

যখন কোডে কোনো ভুল (Error) হয় —তখন PHP যেন চিৎকার করে বন্ধ হয়ে না যায়, বরং শান্তভাবে ভুলটাকে ধরে ফেলতে পারে এবং তুমি ইচ্ছামতো তা হ্যান্ডেল করতে পারো। 
Exception Handling হচ্ছে সেই "ব্রেক" — যেটা দিয়ে তোমার কোড ভুল হলেও থেমে যায় না, সুন্দরভাবে হ্যান্ডেল করে।   

কেন ব্যবহার করা হয়?

```
কারণ	                                                  ব্যাখ্যা
✅ কোড ভেঙে না পড়ে	                                    Error হলে Program বন্ধ না হয়ে graceful ভাবে চলতে পারে
✅ Error Message দেখা যায়	                              কোন Error হলো তা ধরতে পারি
✅ Custom Message/Action	                                  তুমি নিজেই ঠিক করতে পারো, error হলে কী হবে
✅ বড় প্রজেক্টে Safe                                         কোড	User কে সুন্দরভাবে ভুল বোঝানো যায়    
```

উদাহরণ 

```
try {

$result = 10 / 0;
echo $result;
} catch (Throwable $e) {  
    <!-- যদি Error হয়, তাহলে এখানে আসবে | এটাই হল error Handling  -->
    echo "❌ সমস্যা হয়েছে: " . $e->getMessage();
}
```

Exception Handling এর গঠন : 

```
try {
    // যেটা try করা হচ্ছে
} catch (ExceptionType $e) {
    // error হলে এখানে আসে
} finally {
    // সবশেষে যা হোক চলবেই (চাইলে)
}
```

কোড

```
function divide($a, $b) {
    try {
        if ($b == 0) {
            <!-- throw করে exception তৈরি মানে হল এইখানে একটা সমস্যা (error) হয়েছে — এটা উপরে পাঠাও, যেন catch করতে পারি। 
            এই সমস্যার মেসেজ  টা আমি আমার মত করে customize করতে পারছি  -->
            throw new Exception("0 দিয়ে ভাগ করা যায় না!");
        }

        $result = $a / $b;
        echo "ফলাফল: $result <br>";
    } catch (Exception $e) {
        echo "❌ Error: " . $e->getMessage() . "<br>";
    } finally {
        echo "✅ ধন্যবাদ! Divide করার চেষ্টা শেষ।<br><br>";
    }
}

Output হবে:

ফলাফল: 5
✅ ধন্যবাদ! Divide করার চেষ্টা শেষ।

❌ Error: 0 দিয়ে ভাগ করা যায় না!
✅ ধন্যবাদ! Divide করার চেষ্টা শেষ।
```

Line by Line ব্যাখ্যা:
```
অংশ	                                                                  কী করছে
try {}                                                                 এখানে মূল ভাগ করার কাজ করা হচ্ছে
if ($b == 0)	                                                       যদি ভাগের সংখ্যা 0 হয়, তাহলে throw করে exception তৈরি
catch (Exception $e)	                                               এখানে error ধরা হচ্ছে এবং মেসেজ দেখানো হচ্ছে
finally {}	                                                           এটা সবসময়ই চলবে — error হোক বা না হোক

// উদাহরণ
divide(10, 2);   // ঠিক আছে
divide(5, 0);    // Error হবে
```


## SOLID Principles 
SOLID হচ্ছে  OOP-এর ৫টা গুরুত্বপূর্ণ নিয়ম/নীতি। যেটা Software Development-এ code clean, flexible, scalable রাখতে সাহায্য করে।     

### SOLID এর ফুল ফর্ম:

```
Letter	 নাম	                                           মানে
S	     Single Responsibility Principle	               ১টা ক্লাস = ১টা কাজ
O	     Open/Closed Principle	                           কোড পরিবর্তন না করে নতুন ফিচার Add
L	     Liskov Substitution Principle	                   Parent এর জায়গায় Child বসালেও চলবে
I	     Interface Segregation Principle	               ছোট ছোট Interface ব্যবহার করো
D	     Dependency Inversion Principle	                   Abstraction এর উপর ভিত্তি করো, concrete class এর না
```

নিচে এদের নিয়ে বিস্তারিত ভাবে আলোচনা করা হল 

### Single Responsibility Principle (SRP) 
এর অর্থ হচ্ছে ১টা ক্লাসের ১টাই কাজ থাকবে। মানে হচ্ছে ১টা class এর মধ্যে একটা নির্দিষ্ট কাজ গুলো
থাকবে। বিভিন্ন টাইপ এর কাজ একটা class এর মধ্যে না রেখে,একই টাইপ এর কাজ রাখতে হবে। যাতে ক্লাস দেখেই বুজা যায় এখানে কি টাইপের কাজ হয়। 

উদাহরণ :

```
❌ ভুল:
class User {
    public function createUser() {}
    public function sendEmail() {} // আলাদা দায়িত্ব
}
```

```
✅ ঠিক:
class User {
    public function createUser() {}
}

class Email {
    public function sendEmail() {}
    }
```


### OCP = Open/Closed Principle 
"A class should be open for extension, but closed for modification." অর্থাৎ :"তুমি নতুন কিছু যোগ করতে পারো (extend), কিন্তু পুরাতন কোডে হাত দিতে পারবে না (modify না করেই কাজ হবে)।"
আমাদের কোড করার ক্ষেত্রে এমন ভাবে প্ল্যান করে আগাতে হবে যাতে, আমরা কোর ফাঙ্কশন বা পুরাতন কোড এ হাত না দিয়ে নতুন কোড বা ফাঙ্কশন add করতে পারি .

কেন দরকার?
তুমি যখন একটা সফটওয়্যার বানাও, ভবিষ্যতে অনেক সময় নতুন feature যোগ করতে হয়। যদি তুমি বারবার পুরাতন কোডে গিয়ে modify করো, 
তাহলে পুরাতন ফিচার নষ্ট হতে পারে (bug)!এই কারণে OCP কনসেপ্ট টা দরকার .


 উদাহরণ :

 ```
class Invoice {
    public function calculateDiscount($type) {
        if ($type == 'regular') {
            return 5;
        } elseif ($type == 'vip') {
            return 10;
        } elseif ($type == 'supervip') {
            return 15;
        }
    }
}
```
এই কোডে যদি নতুন কোনো type (যেমন: 'student') যোগ করতে চাই, তাহলে:
আমাদের পুরাতন class এর ভিতর গিয়ে কোড modify করতে হবে — যা ভুল! কিন্তু আমরা OCP রুল  অনুসরণ করে অন্য ভাবে কোড করতে পারি,যাতে আমাদের আগের কোড এ হাত দিতে না হয়। 

উদাহরণ :

```
interface Discount {
        public function getDiscount();
    }

    class RegularDiscount implements Discount {
        public function getDiscount() {
            return 5;
        }
    }

    class VipDiscount implements Discount {
        public function getDiscount() {
            return 10;
        }
    }

    class SuperVipDiscount implements Discount {
        public function getDiscount() {
            return 15;
        }
    }

    class Invoice {
        public function calculate(Discount $discount) {
            return $discount->getDiscount();
        }
}
```

বাস্তব উদাহরণ: Laravel-এ OCP Laravel এর অনেক ফিচার (যেমন: Notification channel, Payment gateway) যারা  এই OCP principle টা folow করে।
আমরা চাইলে  নতুন gateway বানাতে পারি , কিন্তু  core যে কোড টুকু আছে ওখানে কিন্তু আমাদের হাত দিতে হয় না। 

### L - Liskov Substitution Principle (LSP) 

এটি SOLID এর তৃতীয় নিয়ম।  Barbara Liskov নামে একজন বিজ্ঞানী এটি প্রস্তাব করেন।"Child class গুলো parent class এর behavior ঠিকঠাকভাবে ধরে রাখবে। 
অর্থাৎ যেখানে parent class use করা হয়, সেখানে তার child class বসালেও সব ঠিকমতো কাজ করবে।" এটাই হল LSP নিয়ম। 
অন্য ভাবে বললে parent class যেটা করার কথা, child class সেটার অন্য রকম আচরণ করলে এটা LSP ভাঙবে ❌
একটা উদাহরণ দিলে বিষয় টা বুজতে সহজ হবে। 


উদাহরণ (LSP নিয়ম মানে না ):

```
class Bird {
    public function fly() {
        echo "Bird is flying 🕊️";
    }
}

class Penguin extends Bird {
    public function fly() {
        throw new Exception("Penguins can't fly!");
    }
}
```


এখানে  Bird class অর্থাৎ parent class বলছে : পাখি উড়তে পারে।
কিন্তু Penguin class বলছে: “Penguins উড়তে পারি না!” । এইখানে child class ,parent class এর বৈশিষ্ঠ ধরে রাখে নেই। বরং child class parent class এর বিপরীত আচরণ করতেছে। 
আর এটাই হচ্ছে LSP violation 

ঠিক পদ্ধতি (LSP মেনে চলে):

```
class Bird {
    public function eat() {
        echo "Bird is eating<br>";
    }
}

class FlyingBird extends Bird {
    public function fly() {
        echo "Flying bird is flying<br>";
    }
}

class Sparrow extends FlyingBird {}
class Penguin extends Bird {} // Fly নাই এখানে — ঠিক আছে!
```

এখানে Bird parent class তাকে extends করে বানানো হয়েছে FlyingBird.আবার FlyingBird কে extends করে Sparrow. এখানে যেটা হচ্ছে Bird খায়, 
FlyingBird খায় এবং উড়ে ,Sparrow খায় এবং উড়ে, ফলে এদের মধ্যে একটা মিল রয়েছে অর্থাৎ parent এবং child class এর মধ্যে একটা মিল রয়েছে। 
ওপর দিকে Penguin যেহেতু উড়ে না ,তাই তাকে FlyingBird extends করে বানানো হয় নাই। তাকে Bird extends করে বানানো হয়েছে। 

মোট কথা হল আমাদের কে parent এবং child class এর মধ্যে মিল রেখে কাজ করতে হবে।     
এটা করলে কী হয়?

Code clean থাকে
Logic mismatch হয় না
Code Reuse সহজ হয়
Bug কম হয়
SOLID principle follow হয়

## Interface Segregation Principle (ISP) 
কোনো class কে এমন interface implement করতে বাধ্য করো না, যেটার সব ফিচার তার দরকার নেই।"অন্য ভাবে "একটা class কে এমন কিছু করতে বাধ্য না করা , যেটা সে জানেই না বা দরকার নাই।"

উদাহরণ :

```
interface Worker {
    public function work();
    public function eat();
}

class Robot implements Worker {
    public function work() {}
    public function eat() {} // Robot তো খায় না!
}
```
এখানে Worker একটা interface যার মধ্যে দুইটা method আছে,আবার Robot class এই Worker interface কে implements করেছে। 
আমরা জানি কোনো class যদি কোনো interface implements করে তাহলে ওই class কে ওই interface এর সব method অব্যশই ব্যবহার করতে হবে। 
এখানে  Robot-কে eat() implement করতে বাধ্য করা হয়েছে — কিন্তু তার ওই কাজ দরকারই নেই!

তাহলে এই same কাজটা যদি ISP follow করে করা হয় সে ক্ষেত্রে code টা হবে। 

```
interface Workable {
    public function work();
}

interface Eatable {
    public function eat();
}

class HumanWorker implements Workable, Eatable {
    public function work() {
        echo "Human working...";
    }
    public function eat() {
        echo "Human eating...";
    }
}

class RobotWorker implements Workable {
    public function work() {
        echo "Robot working...";
    }
}
```
এবার Robot-কে eat() করতে বলা হচ্ছে না, এবার কোড ISP follow করেছে ।


### D — Dependency Inversion Principle (DIP) 
সহজ ভাবে বলতে গেলে উচ্চ স্তরের ক্লাস যেন নিচু স্তরের ক্লাসের উপর নির্ভর না করে। বরং উচ্চ স্তরের ক্লাস  interface বা abstract-এর উপর নির্ভর করবে (একটা নিয়ম মেনে কাজ করবে )।
মোট কথা হচ্ছে উচ্চ স্তরের ক্লাস যেন নিচু স্তরের ক্লাসের উপর নির্ভর না করে ।   
এখন আসি  (High-Level Class বা উচ্চ স্তরের ক্লাস এবং Low-Level Class বা নিচু স্তরের ক্লাস আসলে কি ?

### High-Level Class and Low-Level Class : এটা একটা thinking এর বিষয় , এক এক জন, এক এক ভাবে এটা ভাগ করবে যে কোনটা High-Level Class আর কোনটা  Low-Level Class .এক এক  জনের চিন্তা এক এক রকম হবে। 
তবে কিছু বিষয় এর উপর ভিত্তি করে আমরা একটা guidline করতে পারি যে এটা  High-Level Class এবং এটা  Low-Level Class . 

১.প্রজেক্টের প্রথম দিকে, আমাদের ডিসিশন নিতে হবে যে , কোন পার্ট গুলো আমাদের প্রজেক্ট এর জন্য খুবই গুরথপুর্ণ। 
যেগুলো না থাকলে প্রজেক্ট চালানো যাবে না। আমাদের main business লজিক গুলো। এই জিনিস গুলো যাবে আমাদের high level এ। ধরা যাক e-commerce সাইট। 
একটা e-commerce সাইট এ main বিষয় গুলো কি কি। 

১. user registration
2. product post
3.order management
4. Report
এই বিষয় গুলো আছে বলেই এটা একটা e-commerce সাইট। সর্বনিন্ম এই বিষয় গুলো থাকতে হবে। so এইগুলো বা এই কাজ করার জন্য যে class বেবহার করা হবে সেগুলো হল High-Level Class .

2. যে Class গুলা system-level কাজ করে বা External Resource handle করে
যেমন:
Database access করে [database connection External ]
Email পাঠায় [system-level কারণ  ইমেইল function গুলো করাই থাকে ]
API call করে [External ]
FileUploader[common ]
আরেকটা জিনিস যেটা, প্রায় সব প্রজেক্টই এইগুলো কমন থাকে , এই কাজ গুলো করার জন্য যে  ক্লাস আছে সেগুলো  হচ্ছে  Low-Level Class .মোট কথা হল , 
যেটাই আপনি High-Level ,Low-Level করেন না কেন।  খেয়াল রাখতে হবে High-Level-class  যেন Low-Level-class এর উপর নির্ভর না করে।

উদাহরন : 

```
 <!-- এটা একটা থার্ড পার্টি কাজ , অন্যথায় এটা একটা system-level কাজ , যেটা শুধু পেমেন্ট রিলেটিভ কাজ করে। so বলতেই পারি যে এটা একটা 
                লো-লেভেল class . -->
    class StripePayment {
        public function pay($amount) {
            echo "Paid $amount using Stripe";
        }
    }

    <!-- এটা একটা হাই-লেভেল class  -->
    class OrderManager {
        protected $payment;

        public function __construct() {
            $this->payment = new StripePayment(); // ❌ নির্ভর করছে একটাই payment method এর উপর
        }

        public function placeOrder($amount) {
            $this->payment->pay($amount);
        }
    }
```

এখানে আমরা দেখতে পাচ্ছি একটা একটা হাই-লেভেল class একটা লো-লেভেল class এর উপর নির্ভর করছে। যেটা এই প্রিন্সিপলের rule এর বাহিরে। 

সমস্যা কী?
OrderManager class সরাসরি StripePayment class কে চেনে।
এখন যদি তুমি BkashPayment চালু করতে চাও, তাহলে OrderManager এর কোড change করতে হবে।
এতে code tightly coupled হয়ে গেছে ❌

এবার rule মেনে চলে এরকম একটা উদাহরণ 

```
 <!-- Step 1: একটা Interface তৈরি করি -->
interface PaymentMethod {
    public function pay($amount);
}
<!-- Step 2: এখন Stripe আর Bkash আলাদা আলাদা implement করবে -->
class StripePayment implements PaymentMethod {
    public function pay($amount) {
        echo "Paid $amount using Stripe";
    }
}

class BkashPayment implements PaymentMethod {
    public function pay($amount) {
        echo "Paid $amount using Bkash";
    }
}

<!-- Step 3: এখন High-Level OrderManager class কে interface দেওয়া হবে -->
class OrderManager {
    protected $payment;

    // Constructor Injection
    public function __construct(PaymentMethod $payment) {
        $this->payment = $payment;
    }

    public function placeOrder($amount) {
        $this->payment->pay($amount);
    }
}


<!-- // Stripe দিয়ে পেমেন্ট -->
$order = new OrderManager(new StripePayment());
$order->placeOrder(1000);
// Output: Paid 1000 using Stripe

<!-- // Bkash দিয়ে পেমেন্ট -->
$order2 = new OrderManager(new BkashPayment());
$order2->placeOrder(1500);
// Output: Paid 1500 using Bkash
```


বুঝে নাও এখন:

```
বিষয়	                 DIP না মানলে	                                                 DIP মানলে
পরিবর্তন করলে	         মূল class ভেঙে ফেলতে হয় ❌	                                  শুধু নতুন class বানালেই হয় ✅
Dependency	             class directly depends ❌	                                   interface/abstraction এর উপর depends ✅
Flexibility	             নেই ❌	                                                       অনেক বেশি ✅
```



এইভাবে মনে রাখো:

“High-level manager” যেন সরাসরি “Stripe বা Bkash” (class) এর সাথে কথা না বলে,
বরং একটা “Payment Interface” (interface,abstract) এর মাধ্যমে সবার সাথে কথা বলে।
এটা হলো loose coupling ❤️
এটাই DIP ✅

## Design Patterns 
Design Pattern মানে হলো কিছু "tested & proven" কোডের ধরন বা “solution idea” . 
এক কথায় কোড লেখার একটা ধরণ যা স্বীকৃত এবং টেস্টেড। 
উদাহরণ: আপনি যখন পানি খেতে চান — ১ লিটার বোতলে খাবেন, ২০ লিটারে না।কারণ ছোট বোতল portable. এটাও একরকম “pattern” ।
নিচে Pattern Type এর লিস্ট দেয়া হল 


### Creational Patterns (Object কিভাবে বানাবো)

```
Pattern	                                                 শেখার ধাপ
✅ Singleton	                                           একটাই object থাকবে
✅ Factory	                                           Object তৈরি করবে অন্য class
🔜 Abstract Factory	                                    Factory-র ভিতরে factory
🔜 Builder	                                            ধাপে ধাপে object তৈরি
```

### Structural Patterns (Object গুলা কিভাবে যুক্ত হবে)

```
Pattern	                                     শেখার ধাপ
✅ Adapter	                               এক class কে compatible করা
✅ Decorator	                               নতুন feature যোগ
🔜 Facade	                                Laravel এর Route, Cache এগুলো সব Facade
🔜 Composite	                            Tree structure manage 
``` 

### Behavioral Patterns (Object কিভাবে কথা বলবে/ব্যবহার করবে)

```
Pattern	                              শেখার ধাপ
✅ Observer                     	    Event system → Notify others
✅ Strategy	                        Behavior run time change
🔜 State	                         অবস্থার উপর আচরণ
🔜 Command	                         কাজ গুলো object বানিয়ে রাখা
```

## Singleton 
Singleton হল php একটা ডিসাইন pattern . যার মূল কনসেপ্ট হল। একটা class এর একটাই object (new লিখে যে object তৈরী করি ) থাকবে। 
বার বার new লিখে object তৈরী করা যাবে না। আর এই rule বা pattern টাই হল  Singleton pattern . 
কেন দরকার?
Database Connection — একটাই থাকলেই ভালো

একটা উদাহরণ দিলে বিষয় টা ঠিক ভাবে বুজা যাবে 

```
class Database {
    public static $connection;

    public function __construct() {
        // actual connection বানানো হচ্ছে
        self::$connection = new PDO("mysql:host=localhost;dbname=test", "root", "");
    }
}
$db = new Database 
$db_one  = new Database 
```
এখন এখানে আমি যতবার Database এর object বানাবো (new লিখে) ততবারই নতুন করে  connection খুলবে ,অনেক memory খরচ হবে,
slow performance হবে। এবার যদি আমি Singleton pattern ফলো করে কাজ টা করি তাহলে কি হবে। 

```
class Database {
    private static $connection;

    private function __construct() {
        // actual connection বানানো হচ্ছে
        self::$connection = new PDO("mysql:host=localhost;dbname=test", "root", "");
    }

    public static function getConnection() {
        if (!self::$connection) {
            new self(); // একবারই connection তৈরি হবে
        }
        return self::$connection;
    }
}

$conn = Database::getConnection();
$conn_two  = Database::getConnection();
```

প্রথমত , এখানে আমরা private __construct বেবহার করেছি ফলে ক্লাস এর বাহির থেকে new লিখে object বানানো যাবে না। 
দ্বিতীয়ত , self হল class এর ভিতর যখন ওই class এর property বা method কে access করতে হলে self keyword বেবহার করতে হয়। জাস্ট জানার জন্য 

কোড টা বুজি 
প্রথমত , আমি এখানে new লিখে object বানাতে পারবো না। কারণ এখানে __construct private . আমরা জানি private method class এর বাহির থেকে access করা যায় না। 

 Database::getConnection(); যেহেতু getConnection method টা static তাই একে সরাসরি class দিয়েই access করা যায়। এখানে সেটাই করা হচ্ছে। getConnection call করার পর , প্রথমে method এর ভিতর ঢুকবে এবং দেখবে $connection property ভিতর কিছু আছে কিনা। যদি না থাকে তাহলে সে  new self() [অর্থাৎ class এর  ভিতর থেকে ,এর object তৈরি করা  ] . যখন কোনো class এর object তৈরী করা হয় ,তখন আপনা আপনি __construct মেথড রান বা call হয়। এখানে সেটাই হচ্ছে। এবং  সংগে  সংগে  db connect হইয়া যাবে। 

এখন তুমি যখন Database::getConnection() মেথড টা আবার কল করবে তখন সে মেথড ঢুকবে এবং সে দেখবে self::$connection এ ভ্যালু আছে ফলে সে আর 

```
if (!self::$connection) {
    new self(); // একবারই connection তৈরি হবে
 }
 ```

এখানে ঢুকবে না। ফলাফল new লিখে আর অবজেক্ট তৈরী হবে না।  আর এটাই হচ্ছে Singleton pattern 
Laravel এ কোথায় use হয়?
1.Log
2.config
3.DB
সব singleton instance

## Factory Pattern 
আমরা সাধারণত একটা class এর object (new লিখে ) সরাসরি বানিয়ে কাজ করি। কিন্তু Factory Pattern এর concept হল এই object বানানোর কাজ টা অন্য কোনো method দিয়ে করা। সরাসরি object তৈরী না করা। 

উদাহরণ :

```
interface Toy {
public function play();
}

class ToyCar implements Toy {
public function play() {
    echo "Playing with a 🚗 Car<br>";
}
}

class ToyDrone implements Toy {
public function play() {
    echo "Playing with a 🛸 Drone<br>";
}
}


class ToyFactory {
public static function make($type): Toy {
    if ($type == 'car') {
        return new ToyCar();
    } elseif ($type == 'drone') {
        return new ToyDrone();
    } else {
        throw new Exception("Unknown toy type");
    }
}
}


$toy1 = ToyFactory::make('car');
$toy1->play(); // Output: Playing with a 🚗 Car

$toy2 = ToyFactory::make('drone');
$toy2->play(); // Output: Playing with a 🛸 Drone
```

এখানে আমরা ToyFactory এর make method টা ব্যবহার করেছি object তৈরী করার জন্য। 

 Laravel এ কোথায় use হয়?
1.Laravel service container (app()->make(...))
2.Model factory (User::factory())
3.Database seeder
4.Notification factory
5.Queue Job factory


## Abstract Factory 
অ্যাবস্ট্র্যাক্ট ফ্যাক্টরি প্যাটার্ন হলো একটি ডিজাইন প্যাটার্ন যা আপনাকে একই ধরনের একাধিক অবজেক্টের একটি সম্পূর্ণ সেট (যেমন, একই স্টাইলের আসবাবপত্রের সেট) তৈরি করার জন্য একটি সাধারণ ইন্টারফেস করে  দেয়, 
কিন্তু এটি ক্লায়েন্ট কোডকে সরাসরি জানতে দেয় না যে কোন নির্দিষ্ট ক্লাস ব্যবহার করে সেই অবজেক্টগুলো তৈরি হচ্ছে। 

ধরুন আপনি একটি অ্যাপ্লিকেশন তৈরি করছেন যেখানে দুটি থিম (Theme) আছে: একটি লাইট থিম (Light Theme) এবং একটি ডার্ক থিম (Dark Theme)। 
প্রতিটি থিমের জন্য আপনার একটি বাটন এবং একটি চেক-বক্স দরকার।
এই সমস্যার সমাধান করতে আমরা অ্যাবস্ট্র্যাক্ট ফ্যাক্টরি প্যাটার্ন ব্যবহার করতে পারি।

### ১. Abstract Products (কম্পোনেন্ট ইন্টারফেস)

প্রথমে, আমরা বাটন এবং চেক-বক্সের জন্য দুটি ইন্টারফেস তৈরি করব। এই ইন্টারফেসগুলো বলে দেয় যে প্রতিটি কম্পোনেন্টের কী কী ক্ষমতা থাকতে হবে।

```
// বাটনের জন্য ইন্টারফেস
interface Button {
    public function render();
}

// চেক-বক্সের জন্য ইন্টারফেস
interface Checkbox {
    public function render();
}
```

### ২. Concrete Products (কংক্রিট কম্পোনেন্ট ক্লাস)

এবার আমরা লাইট এবং ডার্ক থিমের জন্য নির্দিষ্ট বাটন এবং চেক-বক্স ক্লাস তৈরি করব।

```
// লাইট থিমের বাটন
class LightButton implements Button {
    public function render() {
        echo "Rendering a light theme button.\n";
    }
}

// লাইট থিমের চেক-বক্স
class LightCheckbox implements Checkbox {
    public function render() {
        echo "Rendering a light theme checkbox.\n";
    }
}

// ডার্ক থিমের বাটন
class DarkButton implements Button {
    public function render() {
        echo "Rendering a dark theme button.\n";
    }
}

// ডার্ক থিমের চেক-বক্স
class DarkCheckbox implements Checkbox {
    public function render() {
        echo "Rendering a dark theme checkbox.\n";
    }
}
```

### ৩. Abstract Factory (মাস্টার ফ্যাক্টরি)

এটি আমাদের মূল ফ্যাক্টরি ইন্টারফেস। এই ইন্টারফেসটি একটি সম্পূর্ণ থিমের কম্পোনেন্ট তৈরি করার জন্য মেথডগুলো ঘোষণা করে।

```
interface UIFactory {
    public function createButton(): Button;
    public function createCheckbox(): Checkbox;
}
```

### ৪. Concrete Factories (কংক্রিট ফ্যাক্টরি)

এই ফ্যাক্টরিগুলো UIFactory ইন্টারফেসকে ইমপ্লিমেন্ট করে এবং নির্দিষ্ট থিমের কম্পোনেন্ট তৈরি করে।

```
// লাইট থিম ফ্যাক্টরি
class LightThemeFactory implements UIFactory {
    public function createButton(): Button {
        return new LightButton();
    }
    public function createCheckbox(): Checkbox {
        return new LightCheckbox();
    }
}

// ডার্ক থিম ফ্যাক্টরি
class DarkThemeFactory implements UIFactory {
    public function createButton(): Button {
        return new DarkButton();
    }
    public function createCheckbox(): Checkbox {
        return new DarkCheckbox();
    }
}
```

### ৫. Client Code (যে কোড ফ্যাক্টরি ব্যবহার করবে)

আমাদের অ্যাপ্লিকেশন কোড (ক্লায়েন্ট কোড) সরাসরি LightButton বা DarkCheckbox ক্লাসকে ব্যবহার করবে না।
এর পরিবর্তে, এটি একটি UIFactory অবজেক্ট গ্রহণ করবে এবং তার মাধ্যমে কম্পোনেন্টগুলো তৈরি করবে।

```
// একটি ফাংশন যা যেকোনো UIFactory ব্যবহার করে UI রেন্ডার করে
function renderUI(UIFactory $factory) {
    $button = $factory->createButton();
    $checkbox = $factory->createCheckbox();

    echo "--- UI কম্পোনেন্ট রেন্ডার হচ্ছে ---\n";
    $button->render();
    $checkbox->render();
    echo "----------------------------------\n";
}

// লাইট থিম ব্যবহার করে UI রেন্ডার করি
echo "লাইট থিমের জন্য UI:\n";
$lightFactory = new LightThemeFactory();
renderUI($lightFactory);

// ডার্ক থিম ব্যবহার করে UI রেন্ডার করি
echo "\nডার্ক থিমের জন্য UI:\n";
$darkFactory = new DarkThemeFactory();
renderUI($darkFactory);
```

### আউটপুট

```
লাইট থিমের জন্য UI:
--- UI কম্পোনেন্ট রেন্ডার হচ্ছে ---
Rendering a light theme button.
Rendering a light theme checkbox.
----------------------------------

ডার্ক থিমের জন্য UI:
--- UI কম্পোনেন্ট রেন্ডার হচ্ছে ---
Rendering a dark theme button.
Rendering a dark theme checkbox.
----------------------------------
```

এই উদাহরণ থেকে আপনি দেখতে পাচ্ছেন:
একই ধরনের অবজেক্টের পরিবার: LightThemeFactory সবসময় একটি LightButton এবং একটি LightCheckbox তৈরি করে, যা একই পরিবারের অংশ।
ক্লায়েন্ট কোডের বিচ্ছিন্নতা: renderUI ফাংশনটি জানে না যে এটি কোন থিমের বাটন বা চেক-বক্স রেন্ডার করছে। এটি শুধু UIFactory ইন্টারফেসের মেথডগুলো ব্যবহার করে, যা কোডকে অত্যন্ত নমনীয় করে তোলে।

### একাধিক অবজেক্টে বলতে কি বুজানো হইছে

"একাধিক অবজেক্টে" বলতে বোঝানো হয়েছে যে, আপনি একই সময়ে একই ধরনের বা সম্পর্কিত একাধিক অবজেক্ট তৈরি করছেন। অ্যাবস্ট্র্যাক্ট ফ্যাক্টরি প্যাটার্নের ক্ষেত্রে, এই অবজেক্টগুলো একটি নির্দিষ্ট পরিবারের সদস্য হয়।
উদাহরণস্বরূপ, যখন আমরা লাইট থিমের জন্য LightThemeFactory ব্যবহার করি, তখন এটি শুধু একটি অবজেক্ট তৈরি করে না, বরং একটি সম্পূর্ণ সেট তৈরি করে:
একটি লাইট থিমের বাটন অবজেক্ট।
একটি লাইট থিমের চেক-বক্স অবজেক্ট।
এখানে, LightButton এবং LightCheckbox হলো সেই একাধিক অবজেক্ট, যারা সবাই লাইট থিম নামক একটি পরিবারের সদস্য। এই অবজেক্টগুলো একে অপরের সাথে সামঞ্জস্যপূর্ণ।
যদি আপনি DarkThemeFactory ব্যবহার করতেন, তাহলে এটিও একাধিক অবজেক্ট তৈরি করত:
একটি ডার্ক থিমের বাটন অবজেক্ট।
একটি ডার্ক থিমের চেক-বক্স অবজেক্ট।
এখানেও, DarkButton এবং DarkCheckbox হলো সেই একাধিক অবজেক্ট, যারা ডার্ক থিম পরিবারের সদস্য।
সুতরাং, "একাধিক অবজেক্ট" বলতে বোঝানো হয়েছে যে, একটি ফ্যাক্টরি ব্যবহার করে আপনি শুধুমাত্র একটি জিনিস নয়, বরং সম্পর্কিত একাধিক জিনিস তৈরি করতে পারছেন, এবং তারা সবাই একই স্টাইল বা ক্যাটাগরির অন্তর্ভুক্ত। এটি নিশ্চিত করে যে আপনার তৈরি করা সিস্টেমের বিভিন্ন অংশগুলো একে অপরের সাথে সামঞ্জস্যপূর্ণ থাকবে।

## Builder Pattern
PHP তে বিল্ডার প্যাটার্ন (Builder Pattern) হলো একটি ডিজাইন প্যাটার্ন যা আপনাকে জটিল অবজেক্ট তৈরি করতে সাহায্য করে। 
এটি এমনভাবে ডিজাইন করা হয়েছে যেন একটি অবজেক্টের প্রতিটি অংশ ধাপে ধাপে তৈরি করা যায়, 
যেখানে প্রতিটি ধাপের জন্য একটি নির্দিষ্ট পদ্ধতি বা মেথড থাকে। এতে করে অবজেক্ট তৈরির প্রক্রিয়াটি সহজ, পরিষ্কার এবং ত্রুটিমুক্ত হয়।

সহজভাবে বলতে গেলে, ধরুন আপনি একটি বার্গার তৈরি করবেন। এই বার্গারে অনেক উপকরণ থাকতে পারে: ব্রেড, প্যাটি, লেটুস, চিজ, সস, ইত্যাদি। 
আপনি যদি সব উপকরণ একবারে মিশিয়ে বার্গার তৈরি করতে যান, তাহলে ভুল হওয়ার সম্ভাবনা থাকে।

বিল্ডার প্যাটার্ন এই সমস্যা সমাধান করে। এটি আপনাকে ধাপে ধাপে বার্গার তৈরি করতে দেয়:
১. প্রথমে ব্রেড নিন।

২. এরপর প্যাটি যোগ করুন।

৩. তারপর লেটুস দিন।

৪. এরপর চিজ দিন।

৫. সবশেষে সস যোগ করুন।

প্রতিটি ধাপের জন্য একটি আলাদা মেথড ব্যবহার করা হয়, যেমন addBread(), addPatty(), addLettuce()। এভাবে আপনি কোন উপাদানটি কখন যোগ করবেন তা নিয়ন্ত্রণ করতে পারেন।

বিল্ডার প্যাটার্নের মূল অংশগুলো
বিল্ডার প্যাটার্নের প্রধানত চারটি অংশ থাকে:

1.Product (প্রোডাক্ট): এটি হলো সেই জটিল অবজেক্ট যা আমরা তৈরি করতে চাই (আমাদের উদাহরণে বার্গার)।

2.Builder (বিল্ডার): এটি হলো একটি ইন্টারফেস বা অ্যাবস্ট্র্যাক্ট ক্লাস যা অবজেক্ট তৈরির ধাপগুলো ঘোষণা করে (যেমন addBread(), addPatty())।

3.ConcreteBuilder (কংক্রিট বিল্ডার): এটি বিল্ডার ইন্টারফেসকে ইমপ্লিমেন্ট করে এবং প্রতিটি ধাপে নির্দিষ্ট অবজেক্ট তৈরি করে। এটি একটি নির্দিষ্ট ধরনের প্রোডাক্ট তৈরি করে (যেমন, একটি ভেজিটেবল বার্গার বা একটি চিকেন বার্গার)।

4.Director (ডিরেক্টর): এটি হলো একটি ক্লাস যা বিল্ডারকে ব্যবহার করে নির্দিষ্ট ক্রম অনুসারে অবজেক্ট তৈরি করে। এটি গ্রাহকের প্রয়োজন অনুযায়ী কোন ধাপে কী করতে হবে তা নির্ধারণ করে।

উদাহরণ: একটি কম্পিউটার তৈরি করা
ধরুন আমরা একটি Computer অবজেক্ট তৈরি করব, যেখানে CPU, RAM, এবং Storage থাকতে পারে।

### ১. Product (Computer ক্লাস)

```
class Computer {
    private $cpu;
    private $ram;
    private $storage;

    public function setCpu($cpu) {
        $this->cpu = $cpu;
    }

    public function setRam($ram) {
        $this->ram = $ram;
    }

    public function setStorage($storage) {
        $this->storage = $storage;
    }

    public function showSpecs() {
        echo "CPU: " . $this->cpu . "\n";
        echo "RAM: " . $this->ram . "\n";
        echo "Storage: " . $this->storage . "\n";
    }
}
```

### ২. Builder (ComputerBuilder ইন্টারফেস)

```
interface ComputerBuilder {
    public function buildCpu();
    public function buildRam();
    public function buildStorage();
    public function getComputer(): Computer;
}
```
### ৩. ConcreteBuilder (GamingComputerBuilder ক্লাস)

```
class GamingComputerBuilder implements ComputerBuilder {
    private $computer;

    public function __construct() {
        $this->computer = new Computer();
    }

    public function buildCpu() {
        $this->computer->setCpu("Intel Core i9");
    }

    public function buildRam() {
        $this->computer->setRam("32GB DDR5");
    }

    public function buildStorage() {
        $this->computer->setStorage("1TB NVMe SSD");
    }

    public function getComputer(): Computer {
        return $this->computer;
    }
}
```

### ৪. Director (ComputerDirector ক্লাস)

```
class ComputerDirector {
    public function build(ComputerBuilder $builder) {
        $builder->buildCpu();
        $builder->buildRam();
        $builder->buildStorage();
    }
}
```

### ডিরেক্টর এখানে নির্দিষ্ট ক্রম অনুসারে বিল্ডারকে বলে দিচ্ছে কোন অংশটি কখন তৈরি করতে হবে।
ব্যবহার (Client Code)

```
// একটি ডিরেক্টর তৈরি করি
$director = new ComputerDirector();

// একটি গেমিং কম্পিউটার বিল্ডার তৈরি করি
$gamingBuilder = new GamingComputerBuilder();

// ডিরেক্টরের মাধ্যমে গেমিং কম্পিউটার তৈরি করি
$director->build($gamingBuilder);

// তৈরি হওয়া কম্পিউটারটি পাই
$gamingComputer = $gamingBuilder->getComputer();

// স্পেসিফিকেশন দেখি
$gamingComputer->showSpecs();
```

### আউটপুট:

```
CPU: Intel Core i9
RAM: 32GB DDR5
Storage: 1TB NVMe SSD
```

### কেন বিল্ডার প্যাটার্ন ব্যবহার করবেন?

জটিলতা হ্রাস: এটি জটিল অবজেক্ট তৈরির প্রক্রিয়াকে সহজ ও ধাপে ধাপে বিভক্ত করে।
নমনীয়তা: আপনি একই বিল্ডিং প্রক্রিয়ায় ভিন্ন ধরনের বিল্ডার ব্যবহার করে ভিন্ন ধরনের অবজেক্ট তৈরি করতে পারেন। যেমন, আপনি একটি OfficeComputerBuilder তৈরি করে কম শক্তিশালী উপাদান ব্যবহার করতে পারেন।
পঠনযোগ্যতা: কোড অনেক বেশি পঠনযোগ্য এবং পরিষ্কার হয়, কারণ প্রতিটি ধাপের উদ্দেশ্য স্পষ্ট।
ইমিউটেবল অবজেক্ট: এটি আপনাকে ইমিউটেবল অবজেক্ট তৈরি করতে সাহায্য করে, কারণ অবজেক্টটি সম্পূর্ণ তৈরি হওয়ার পরই ব্যবহার করা যায়।


## Adapter Pattern

PHP তে অ্যাডাপ্টার প্যাটার্ন (Adapter Pattern) হলো একটি ডিজাইন প্যাটার্ন যা দুটি ভিন্ন ইন্টারফেস বা ক্লাসের মধ্যে কাজ করতে সাহায্য করে। 
এটি এমনভাবে কাজ করে যেন দুটি বেমানান জিনিস একে অপরের সাথে কথা বলতে পারে। সহজ ভাষায়, একটি অ্যাডাপ্টার প্যাটার্ন একটি কনভার্টারের (Converter) মতো কাজ করে। 

👉 ধরো, তোমার কাছে একটা পুরোনো চার্জার আছে (৩-পিন), কিন্তু তোমার নতুন মাল্টি-প্লাগে শুধু ২-পিন ঢোকে।
➡️ এখন তুমি সরাসরি চার্জার লাগাতে পারছো না।
➡️ তুমি একটা অ্যাডাপ্টার ব্যবহার করলে, যেটা ৩-পিনকে ২-পিনে কনভার্ট করে দিলো।

### অ্যাডাপ্টার প্যাটার্নের মূল অংশগুলো:

Target (টার্গেট): এটি হলো সেই ইন্টারফেস যা ক্লায়েন্ট কোড ব্যবহার করতে চায়। এটি একটি নতুন ইন্টারফেস যা আপনি ব্যবহার করতে চান।
Adaptee (অ্যাডাপ্টি): এটি হলো সেই ক্লাস যা আপনার কাছে বিদ্যমান এবং যা অ্যাডাপ্ট করা প্রয়োজন। এর ইন্টারফেসটি টার্গেটের সাথে সামঞ্জস্যপূর্ণ নয়।
Adapter (অ্যাডাপ্টার): এটি হলো সেই ক্লাস যা টার্গেট ইন্টারফেসকে ইমপ্লিমেন্ট করে এবং অ্যাডাপ্টি অবজেক্টকে ধারণ করে। এটি দুটি ইন্টারফেসের মধ্যে সংযোগ স্থাপন করে।

### সহজ উদাহরণ (PHP কোডে)

১. পুরোনো ক্লাস (Adaptee)

```
// পুরোনো ক্লাস যা temperature ফারেনহাইটে দেয়
class OldWeatherService {
    public function getTemperatureFahrenheit(): float {
        return 98.6; // ফারেনহাইটে টেম্পারেচার
    }
}
```

২. নতুন সিস্টেম (Target)

```
// আমাদের নতুন সিস্টেম temperature সেলসিয়াসে চায়
interface NewWeatherService {
    public function getTemperatureCelsius(): float;
}
```

৩. Adapter

```
class WeatherAdapter implements NewWeatherService {
    private $oldService;

    public function __construct(OldWeatherService $oldService) {
        $this->oldService = $oldService;
    }

    public function getTemperatureCelsius(): float {
        $f = $this->oldService->getTemperatureFahrenheit();
        return ($f - 32) * 5/9; // ফারেনহাইট থেকে সেলসিয়াসে রূপান্তর
    }
}
```

৪. ব্যবহার

```
$oldService = new OldWeatherService();
$adapter = new WeatherAdapter($oldService);

echo "Temperature: " . $adapter->getTemperatureCelsius() . " °C";
```

✅ আউটপুট হবে →

```
Temperature: 37 °C
```

### সারসংক্ষেপ

Target (আমরা যা চাই): NewWeatherService → সেলসিয়াসে টেম্পারেচার
Adaptee (যা আছে): OldWeatherService → ফারেনহাইটে টেম্পারেচার
Adapter (মাঝের লোক): WeatherAdapter → ফারেনহাইটকে সেলসিয়াসে কনভার্ট করে দেয়

সহজ কথায় –
Adapter Pattern = যখন তোমার পুরোনো ক্লাস বা কোড সরাসরি কাজে লাগে না, তখন একটা অ্যাডাপ্টার ক্লাস বানিয়ে নতুন সিস্টেমের সাথে মানিয়ে নাও।


## Decorator Pattern

Decorator Pattern হলো এমন একটি Design Pattern,
যেখানে আমরা কোনো class এর মূল structure না বদলিয়ে,
runtime এ নতুন feature / behavior যোগ করি।

আরেকটু অন্য ভাবে বলতে গেলে 

প্যাটার্ন হলো একটি ডিজাইন প্যাটার্ন যা একটি অবজেক্টের কার্যকারিতা বা আচরণকে গতিশীলভাবে (dynamically) প্রসারিত করতে সাহায্য করে, কোনো নির্দিষ্ট ক্লাস পরিবর্তন না করেই। এটি এমনভাবে কাজ করে যেন আপনি একটি অবজেক্টকে একটি প্যাকেজের মতো মোড়ক (wrap) করতে পারেন এবং প্রতিটি নতুন মোড়ক একটি নতুন বৈশিষ্ট্য যোগ করে। 

সহজ ভাষায়, ধরুন আপনি একটি সাধারণ কফি তৈরি করেছেন। এখন আপনি এই কফিতে অতিরিক্ত বৈশিষ্ট্য যোগ করতে চান, যেমন:
১.প্রথমে কফিতে দুধ যোগ করলেন।
২.তারপর চিনির পরিবর্তে মধু যোগ করলেন।
৩.সবশেষে উপরে ক্রিম যোগ করলেন।

আপনি কফির মূল অবজেক্টকে পরিবর্তন না করে এই অতিরিক্ত বৈশিষ্ট্যগুলো একে একে যোগ করেছেন। প্রতিটি নতুন উপাদান (দুধ, মধু, ক্রিম) হলো একটি সাজসজ্জা (decoration) যা কফিকে নতুন বৈশিষ্ট্য দিয়েছে।

Decorator প্যাটার্ন এই কাজটিই করে। এটি একটি অবজেক্টকে অন্য একটি অবজেক্টের মধ্যে রাখে, যা মূল অবজেক্টের মেথডগুলো কল করার আগে বা পরে অতিরিক্ত কিছু কাজ করে।

### Decorator প্যাটার্নের মূল অংশগুলো

1.Component Interface (কম্পোনেন্ট ইন্টারফেস): এটি একটি সাধারণ ইন্টারফেস যা মূল অবজেক্ট এবং সব ডেকোরেটর ক্লাসকে বাস্তবায়ন করতে হবে। এটি সব অবজেক্টের জন্য একটি সাধারণ কাঠামো সরবরাহ করে।

2.Concrete Component (কংক্রিট কম্পোনেন্ট): এটি হলো সেই মূল ক্লাস যার কার্যকারিতা আমরা প্রসারিত করতে চাই। এটি কোনো অতিরিক্ত বৈশিষ্ট্য ছাড়াই সাধারণ অবজেক্ট।

3.Decorator Base Class (ডেকোরেটর বেস ক্লাস): এটি একটি অ্যাবস্ট্র্যাক্ট ক্লাস যা কম্পোনেন্ট ইন্টারফেসকে বাস্তবায়ন করে এবং একটি কম্পোনেন্ট অবজেক্টকে ধারণ করে। এটি নিশ্চিত করে যে সব ডেকোরেটর একই কাঠামোর। এখানে কম্পোনেন্ট object টা হল BasicPizza

4.Concrete Decorator (কংক্রিট ডেকোরেটর): এটি হলো সেই ক্লাস যা ডেকোরেটর বেস ক্লাস থেকে এক্সটেন্ড করে এবং একটি নির্দিষ্ট অতিরিক্ত বৈশিষ্ট্য যোগ করে।

### উদাহরণ: পিৎজা তৈরি করা

ধরুন আপনি একটি সাধারণ পনিরের পিৎজা তৈরি করবেন এবং এতে অতিরিক্ত টপিং যোগ করে এর দাম এবং বর্ণনা পরিবর্তন করবেন।

Component Interface (পিৎজা ইন্টারফেস)
এই ইন্টারফেসটি আমাদের পিৎজার মূল কাঠামো নির্ধারণ করে, যা ডেকোরেটর এবং মূল ক্লাস উভয়ের জন্য সাধারণ।

```
interface Pizza {
    public function getPrice(): float;
    public function getDescription(): string;
}
```

Concrete Component (সাধারণ পিৎজা ক্লাস)
এটি আমাদের মূল পিৎজা অবজেক্ট, যা কোনো অতিরিক্ত টপিং ছাড়াই।

```
class BasicPizza implements Pizza {
    public function getPrice(): float {
        return 10.0;
    }
    public function getDescription(): string {
        return "Simple Pizza";
    }
}
```

Decorator Base Class (পিৎজা ডেকোরেটর)
এটি একটি অ্যাবস্ট্র্যাক্ট ডেকোরেটর ক্লাস যা Pizza ইন্টারফেসকে বাস্তবায়ন করে।

```
abstract class PizzaDecorator implements Pizza {
    protected $pizza;

    public function __construct(Pizza $pizza) {
        $this->pizza = $pizza;
    }

    // এই মেথডগুলো ডেকোরেটরের উপক্লাসগুলো ওভাররাইড করবে
    public function getPrice(): float {
        return $this->pizza->getPrice();
    }
    public function getDescription(): string {
        return $this->pizza->getDescription();
    }
}
```

Concrete Decorator (টপিং ক্লাস)
এগুলো হলো সেই ডেকোরেটর ক্লাস যা অতিরিক্ত টপিং যোগ করবে এবং দাম ও বিবরণ পরিবর্তন করবে।

```
class CheeseTopping extends PizzaDecorator {
    public function getPrice(): float {
        return $this->pizza->getPrice() + 2.0;
    }
    public function getDescription(): string {
        return $this->pizza->getDescription() . ", extra cheese";
    }
}

class PepperoniTopping extends PizzaDecorator {
    public function getPrice(): float {
        return $this->pizza->getPrice() + 3.5;
    }
    public function getDescription(): string {
        return $this->pizza->getDescription() . ", pepperoni";
    }
}
```

ব্যবহার (Client Code)
এখন আমরা একটি সাধারণ পিৎজা তৈরি করে তাতে অতিরিক্ত টপিং যোগ করব।

```
// একটি সাধারণ পিৎজা তৈরি করি
$myPizza = new BasicPizza();
echo "Your order: " . $myPizza->getDescription() . "\n";
echo "Total Price: $" . $myPizza->getPrice() . "\n";
echo "------------------------------\n";

// পিৎজাতে এক্সট্রা চিজ যোগ করি
$myPizza = new CheeseTopping($myPizza);
echo "Your order: " . $myPizza->getDescription() . "\n";
echo "Total Price: $" . $myPizza->getPrice() . "\n";
echo "------------------------------\n";

// পিৎজাতে পেপারনি যোগ করি
$myPizza = new PepperoniTopping($myPizza);
echo "Your order: " . $myPizza->getDescription() . "\n";
echo "Total Price: $" . $myPizza->getPrice() . "\n";
```

আউটপুট:

```
Your order: Simple Pizza
Total Price: $10

------------------------------
Your order: Simple Pizza, extra cheese
Total Price: $12

------------------------------
Your order: Simple Pizza, extra cheese, pepperoni
Total Price: $15.5
```

### কেন Decorator প্যাটার্ন ব্যবহার করবেন?
ওপেন/ক্লোজড প্রিন্সিপল (Open/Closed Principle): এটি আপনাকে বিদ্যমান ক্লাস (যেমন BasicPizza) পরিবর্তন না করেই নতুন কার্যকারিতা যোগ করতে দেয়। আপনি নতুন ডেকোরেটর তৈরি করে সহজেই নতুন টপিং যোগ করতে পারেন।

নমনীয়তা: আপনি যেকোনো ডেকোরেটরকে যেকোনো ক্রমে ব্যবহার করতে পারেন। আপনি আপনার প্রয়োজন অনুযায়ী একটি পিৎজায় বিভিন্ন টপিং যোগ করতে পারেন।

বিকল্প হিসেবে: এটি সাবক্লাসিং (subclassing) এর একটি বিকল্প। যদি আপনি প্রতিটি সম্ভাব্য টপিং কম্বিনেশনের জন্য সাবক্লাস তৈরি করতে যান, তাহলে ক্লাসের সংখ্যা অনেক বেড়ে যাবে। Decorator প্যাটার্ন এই সমস্যাটি সমাধান করে।

### Decorator Base Class এর ভূমিকা


Decorator Base Class একটি টেমপ্লেট বা ছাঁচের মতো কাজ করে। এর মূল কাজ হলো:

1.সাধারণ কাঠামোর নিশ্চয়তা (Guarantees Common Structure): এটি নিশ্চিত করে যে সব ডেকোরেটর ক্লাস (যেমন, আমাদের পিৎজার উদাহরণে CheeseTopping বা PepperoniTopping) একই ধরনের মেথড (getPrice(), getDescription()) ব্যবহার করবে। এটি একটি সাধারণ কাঠামো তৈরি করে যা সব ডেকোরেটরকে অনুসরণ করতে হয়।

2.অবজেক্ট ধারণ করা (Holds the Wrapped Object): Decorator Base Class এর ভেতরে একটি সুরক্ষিত (protected) প্রপার্টি থাকে যা মূল অবজেক্ট (আমাদের উদাহরণে Pizza অবজেক্ট) ধারণ করে। এটি এমন একটি বাক্সর মতো, যার ভেতরে আসল জিনিসটি রাখা হয়।

3.ডেলিগেশন (Delegation): এটি মেথড কলগুলোকে মূল অবজেক্টের কাছে পাঠিয়ে দেয়। অর্থাৎ, যদি কোনো ডেকোরেটরের মেথড কল করা হয়, এবং সেই ডেকোরেটরটি সরাসরি কোনো অতিরিক্ত কাজ না করে, তাহলে এটি সেই মেথড কলটি মূল অবজেক্টের কাছে পাঠিয়ে দেয়। এটি নিশ্চিত করে যে মূল অবজেক্টের কার্যকারিতা সংরক্ষিত থাকে।

### আমাদের উদাহরণে Pizza অবজেক্টধা ধারণ করে।  এখানে pizza object না interface 

আপনার প্রশ্নটি খুবই সঠিক এবং গুরুত্বপূর্ণ। এখানে একটি সূক্ষ্ম কিন্তু গুরুত্বপূর্ণ পার্থক্য আছে।

আপনার দেওয়া কথাটি: "আমাদের উদাহরণে Pizza অবজেক্ট ধারণ করে" - এটি আংশিকভাবে সঠিক।

সঠিকভাবে বলতে গেলে, PizzaDecorator ক্লাসটি একটি অবজেক্ট ধারণ করে, কিন্তু সেই অবজেক্টটি Pizza ইন্টারফেসকে ইমপ্লিমেন্ট করে।

কেন এই পার্থক্যটি গুরুত্বপূর্ণ?
১.  ইন্টারফেস (Interface) হলো একটি চুক্তি: Pizza ইন্টারফেসটি একটি চুক্তি বা ব্লুপ্রিন্ট। এটি বলে দেয় যে, যে কোনো ক্লাস যদি এই ইন্টারফেসটি ব্যবহার করে, তাহলে সেই ক্লাসের অবশ্যই getPrice() এবং getDescription() মেথডগুলো থাকতে হবে।

২.  অবজেক্ট (Object) হলো বাস্তবায়ন: BasicPizza বা CheeseTopping হলো সেই ক্লাস যারা Pizza ইন্টারফেসকে বাস্তবায়ন করে এবং তাদের নিজস্ব অবজেক্ট তৈরি করা যায়।

PizzaDecorator এর কনস্ট্রাক্টরটি Pizza $pizza টাইপ হিন্ট ব্যবহার করে। এর অর্থ হলো, এই কনস্ট্রাক্টরটি শুধুমাত্র এমন একটি অবজেক্ট গ্রহণ করবে যা Pizza ইন্টারফেসের চুক্তি মেনে চলে।

উদাহরণে এর প্রয়োগ
যখন আপনি এই কোডটি লেখেন:

```
$myPizza = new BasicPizza();
$myPizza = new CheeseTopping($myPizza);
```

এখানে:

প্রথম লাইনে, $myPizza ভেরিয়েবলটি একটি BasicPizza অবজেক্ট ধারণ করে।

দ্বিতীয় লাইনে, $myPizza কে CheeseTopping এর কনস্ট্রাকটরে পাস করা হয়। যেহেতু BasicPizza ক্লাসটি Pizza ইন্টারফেসকে ইমপ্লিমেন্ট করে, তাই এটি CheeseTopping এর জন্য একটি বৈধ প্যারামিটার।

CheeseTopping এর ভেতরে $this->pizza প্রপার্টিটি এখন BasicPizza অবজেক্টটিকে ধারণ করে।

সুতরাং, PizzaDecorator আসলে একটি কংক্রিট অবজেক্টকে (যেমন BasicPizza) ধারণ করে, কিন্তু এটি নির্ভর করে তার ইন্টারফেসের উপর (Pizza)। এটাই এই প্যাটার্নের মূল শক্তি, কারণ এটি ডেকোরেটরকে যেকোনো Pizza অবজেক্টের সাথে কাজ করার স্বাধীনতা দেয়, সেটি BasicPizza হোক বা অন্য কোনো ডেকোরেটর।

## Facade Pattern

Facade Pattern হলো এমন একটা Design Pattern,
যা জটিল সিস্টেমকে সহজ interface দিয়ে ব্যবহার করার সুযোগ দেয়।

Facade Pattern হলো এমন একটা Design Pattern,
যা জটিল সিস্টেম বা একাধিক class কে সহজে ভাবে ব্যবহার করার জন্য একটা interface তৈরি করে দেয়। 

বাংলায় 'ইন্টারফেস' (Interface) এর অর্থ হলো সংযোগের মাধ্যম বা সংযোগস্থল। এটি এমন একটি প্ল্যাটফর্ম বা সীমানা, যা দুটি ভিন্ন সিস্টেম, ডিভাইস, সফটওয়্যার বা ব্যবহারকারীর মধ্যে যোগাযোগ এবং তথ্য বিনিময়ের সুযোগ করে দেয়। এ

মানে, ভেতরে অনেকগুলো class/method থাকলেও,
ইউজারকে শুধু একটাই দরজা (Facade) দিয়ে কাজ করতে হয়।

### সহজ উদাহরণ (বাস্তব জীবন থেকে)


একটি বাস্তব জীবনের উদাহরণ দিলে বিষয়টি পরিষ্কার হবে। ধরুন আপনি একটি স্মার্ট হোম সিস্টেম ব্যবহার করছেন। এই সিস্টেমে বিভিন্ন ডিভাইস আছে: লাইট, টেলিভিশন, সাউন্ড সিস্টেম, এয়ার কন্ডিশনার ইত্যাদি। একটি সিনেমা দেখতে হলে আপনাকে প্রতিটি ডিভাইস আলাদাভাবে অন করতে হবে, যেমন:
১.  লাইট বন্ধ করো।
২.  টিভি অন করো।
৩.  সাউন্ড সিস্টেম অন করো।
৪.  এয়ার কন্ডিশনার অন করো।
এই প্রক্রিয়াটি বেশ জটিল। কিন্তু একটি Facade থাকলে আপনি শুধু একটি বাটন চাপবেন, যার নাম watchMovie()। এই একটি মেথডই ভেতরের সব জটিল কাজগুলো স্বয়ংক্রিয়ভাবে করে দেবে। Facade প্যাটার্ন ঠিক এই কাজটিই করে। এটি একটি সহজ ইন্টারফেসের মাধ্যমে একাধিক ক্লাসের জটিল প্রক্রিয়াগুলোকে আড়াল করে।

### Facade প্যাটার্নের মূল অংশগুলো
1.Facade (ফেসাদ): এটি হলো সেই ক্লাস যা ক্লায়েন্টকে একটি সরল ইন্টারফেস সরবরাহ করে। এটি একটি বা একাধিক সাবসিস্টেম ক্লাসের সাথে কাজ করে এবং ক্লায়েন্টের অনুরোধগুলো সেই ক্লাসগুলোতে পাঠায়।
2.Subsystem Classes (সাবসিস্টেম ক্লাস): এগুলো হলো সেই জটিল ক্লাসগুলো যা ফেসাদ ক্লাস তার অভ্যন্তরীণ কাজগুলো সম্পন্ন করার জন্য ব্যবহার করে। এই ক্লাসগুলো ফেসাদ সম্পর্কে কিছু জানে না।
3.Client (ক্লায়েন্ট): এটি হলো সেই কোড যা ফেসাদ ক্লাসকে ব্যবহার করে। ক্লায়েন্ট সাবসিস্টেমের জটিলতা সম্পর্কে কিছুই জানে না।


### উদাহরণ: একটি ই-কমার্স অর্ডার সিস্টেম
ধরুন আপনার একটি ই-কমার্স ওয়েবসাইট আছে। যখন একজন গ্রাহক একটি অর্ডার দেন, তখন অনেকগুলো প্রক্রিয়া সম্পন্ন হয়:

1.ইনভেন্টরি চেক করা।
2.পেমেন্ট প্রসেস করা।
3.শিপিং নিশ্চিত করা।

এই প্রতিটি কাজের জন্য একটি করে আলাদা ক্লাস রয়েছে। Facade প্যাটার্ন ব্যবহার করে আমরা এই প্রক্রিয়াগুলোকে একটি মাত্র মেথডের অধীনে নিয়ে আসতে পারি।

১.Subsystem Classes (সাবসিস্টেম ক্লাস)
এগুলো হলো সেই জটিল ক্লাসগুলো যা একটি অর্ডার প্রক্রিয়াকরণের জন্য প্রয়োজন।

```
class InventorySystem {
    public function checkStock($productId): bool {
        echo "Checking inventory for product: " . $productId . "\n";
        return true; // ধরুন স্টক আছে
    }
}

class PaymentGateway {
    public function processPayment($amount): bool {
        echo "Processing payment of $" . $amount . "\n";
        return true; // ধরুন পেমেন্ট সফল
    }
}

class ShippingSystem {
    public function scheduleDelivery($address) {
        echo "Scheduling delivery to: " . $address . "\n";
    }
}
```

২.Facade (ফেসাদ)
এই ক্লাসটি একটি সাধারণ ইন্টারফেস সরবরাহ করবে যা উপরের সব ক্লাসকে ব্যবহার করবে।

```
class OrderFacade {
    private $inventory;
    private $payment;
    private $shipping;

    public function __construct() {
        $this->inventory = new InventorySystem();
        $this->payment = new PaymentGateway();
        $this->shipping = new ShippingSystem();
    }

    public function placeOrder($productId, $amount, $address): bool {
        echo "Starting to place an order...\n";

        if (!$this->inventory->checkStock($productId)) {
            echo "Failed: Product is out of stock.\n";
            return false;
        }

        if (!$this->payment->processPayment($amount)) {
            echo "Failed: Payment processing failed.\n";
            return false;
        }

        $this->shipping->scheduleDelivery($address);
        echo "Order placed successfully!\n";
        return true;
    }
}
```
৩.Client (ক্লায়েন্ট)
ক্লায়েন্ট কোডটি এখন শুধু OrderFacade ক্লাস ব্যবহার করবে এবং এর ভেতরের জটিলতা সম্পর্কে কিছুই জানবে না।

```
// একটি অর্ডার ফেসাদ তৈরি করি
$orderFacade = new OrderFacade();

// একটি মাত্র মেথড কল করে পুরো অর্ডার প্রক্রিয়া সম্পন্ন করি
$orderFacade->placeOrder("P001", 150.00, "123 Main St, Anytown");
```

আউটপুট:

```
Starting to place an order...
Checking inventory for product: P001
Processing payment of $150
Scheduling delivery to: 123 Main St, Anytown
Order placed successfully!
```

এই উদাহরণে, ক্লায়েন্টকে ইনভেন্টরি, পেমেন্ট, বা শিপিং ক্লাস সম্পর্কে জানতে হচ্ছে না। সে শুধু OrderFacade ক্লাসের placeOrder() মেথডটি কল করে পুরো কাজটি সম্পন্ন করতে পারছে। এটিই Facade প্যাটার্নের মূল উদ্দেশ্য।

## Composite Pattern

কম্পোজিট প্যাটার্ন এমন একটি কৌশল যা আপনাকে একটি একক জিনিস এবং অনেকগুলো জিনিসের একটি গ্রুপকে একই পদ্ধতিতে ব্যবহার করতে সাহায্য করে। এর মূল উদ্দেশ্য হলো: আপনি একক জিনিস এবং গ্রুপ উভয়কেই একই নামে বা একই কমান্ড দিয়ে নিয়ন্ত্রণ করতে পারবেন।

একটি বাস্তব জীবনের উদাহরণ দিয়ে বুঝি। ধরুন আপনার কম্পিউটার বা মোবাইলে একটি ফাইল সিস্টেম আছে।

এখানে একটি একক ফাইল (যেমন, photo.jpg) আছে।

আবার একটি ফোল্ডারও (যেমন, My_Pictures) আছে, যার ভিতরে অনেকগুলো ফাইল এবং ফোল্ডার থাকতে পারে।

আপনি যদি একটি ফাইল ওপেন করতে চান, আপনি open() কমান্ড ব্যবহার করেন। আবার, আপনি যদি একটি ফোল্ডারের ভেতরকার সবকিছু দেখতে চান, আপনি একই open() কমান্ড ব্যবহার করতে পারেন। ফাইল এবং ফোল্ডার দুটি ভিন্ন ধরনের জিনিস হলেও আপনি তাদের সাথে একই ধরনের আচরণ করতে পারছেন।

কম্পোজিট প্যাটার্ন এই লজিকটিই ব্যবহার করে। এটি একটি সাধারণ কাঠামো (যেমন, FileComponent) তৈরি করে যা উভয়কেই (ফাইল এবং ফোল্ডার) ধারণ করে।

### মূল অংশগুলো:

কম্পোনেন্ট (Component): এটি হলো সেই সাধারণ কাঠামো, যা বলে দেয় যে ফাইল এবং ফোল্ডার উভয়েরই কী কী ক্ষমতা থাকতে হবে। আমাদের উদাহরণে, এটি হলো FileComponent ইন্টারফেস যার একটি মেথড আছে, যেমন display(), যা ফাইল এবং ফোল্ডার উভয়কেই কিছু তথ্য দেখাবে।

পাতা (Leaf): এটি হলো সবচেয়ে মৌলিক উপাদান। এটি একটি একক ফাইল, যার কোনো শিশু উপাদান নেই। যেমন, TextFile বা ImageFile।

গ্রুপ (Composite): এটি হলো একটি গ্রুপ অবজেক্ট যা শিশু উপাদান ধারণ করে। এটি একটি ফোল্ডারের মতো, যার ভেতরে অন্যান্য ফাইল এবং ফোল্ডার থাকতে পারে। যেমন, Folder ক্লাস।


### কেন এই প্যাটার্নটি দরকার?
যদি আপনার কম্পোজিট প্যাটার্ন না থাকতো, তাহলে আপনাকে বারবার চেক করতে হতো যে আপনি একটি ফাইল নিয়ে কাজ করছেন নাকি একটি ফোল্ডার নিয়ে।

### উদাহরণ

```
<?php
Component (কম্পোনেন্ট): এটি হলো একটি সাধারণ ইন্টারফেস, যা ফাইল এবং ফোল্ডার উভয়ের জন্য একটি সাধারণ কাঠামো সরবরাহ করে। এখানে, এটি হলো FileSystemComponent।

interface FileSystemComponent {
    public function showDetails(string $indent = "");
}


Leaf (পাতা): এটি হলো সবচেয়ে মৌলিক উপাদান, অর্থাৎ একটি একক ফাইল। এর ভেতরে কোনো শিশু উপাদান নেই।

class File implements FileSystemComponent {
    private $name;

    public function __construct(string $name) {
        $this->name = $name;
    }

    public function showDetails(string $indent = "") {
        echo $indent . "File44: " . $this->name . "\n";
    }
}


Composite (কম্পোজিট): এটি হলো একটি গ্রুপ যা অন্য ফাইল বা ফোল্ডার ধারণ করতে পারে। এটি একটি ফোল্ডারের মতো কাজ করে।

class Folder implements FileSystemComponent {
    private $name;
    private $components = [];

    public function __construct(string $name) {
        $this->name = $name;
    }

    public function add(FileSystemComponent $component) {
        $this->components[] = $component;
    }

    public function showDetails(string $indent = "") {
      
    

        echo $indent . "Folder: " . $this->name . "\n";
        $newIndent = $indent . "  "; //Indentation for sub-items
      
        foreach ($this->components as $component) {
            $component->showDetails($newIndent);
        }
    }
}

ব্যবহার (ক্লায়েন্ট কোড)
এবার দেখুন, কীভাবে একটি মাত্র কমান্ড দিয়ে আমরা পুরো কাঠামোটি নিয়ন্ত্রণ করতে পারি।


// ফাইল তৈরি করি
$file1 = new File("resume.pdf");
$file2 = new File("photo.jpg");
$file3 = new File("document.txt");

// ফোল্ডার তৈরি করি
$documentsFolder = new Folder("Documents");
$imagesFolder = new Folder("Images");

// ফোল্ডারের মধ্যে ফাইল যুক্ত করি
$documentsFolder->add($file1);
$imagesFolder->add($file2);

// মূল ফোল্ডার তৈরি করি
$myDrive = new Folder("My Drive");

// মূল ফোল্ডারে ফাইল এবং ফোল্ডার উভয়ই যুক্ত করি
$myDrive->add($documentsFolder);
$myDrive->add($imagesFolder);
$myDrive->add($file3); // এখানে একটি একক ফাইল যুক্ত করা হয়েছে

// পুরো ফাইল সিস্টেমটি একটি মাত্র কমান্ড দিয়ে প্রদর্শন করি
$myDrive->showDetails();
?>


output:
Folder: My Drive
  Folder: Documents
    File44: resume.pdf
  Folder: Images
    File44: photo.jpg
  File44: document.txt
```


## Observer Pattern
Observer Pattern হলো এমন একটা ডিজাইন প্যাটার্ন,
যেখানে একটা অবজেক্ট (Subject)-এ কোনো পরিবর্তন হলে,
তার সাথে যুক্ত থাকা অনেকগুলো অবজেক্ট (Observers)-কে স্বয়ংক্রিয়ভাবে জানানো হয়।

এটি এমনভাবে কাজ করে যে, যখন একটি অবজেক্টের অবস্থা (state) পরিবর্তিত হয়, তখন স্বয়ংক্রিয়ভাবে এর উপর নির্ভরশীল সব অবজেক্টকে জানিয়ে দেওয়া হয়, কিন্তু সেই অবজেক্টগুলো একে অপরের সম্পর্কে কিছু জানে না।

মানে 
একজন শিক্ষক (Subject) ক্লাসে ঢুকে বললেন "আজ পরীক্ষা হবে"।
সব ছাত্র (Observers) সেই মেসেজটা শুনে ফেলল।
শিক্ষক আলাদা আলাদা করে প্রত্যেক ছাত্রকে বলেননি।


### Observer Pattern এর প্রধান অংশ

1️⃣ Subject (বা Publisher)

যেটা change/event তৈরি করে।
এর কাজ হলো observer-দের list মেইনটেইন করা, আর পরিবর্তন হলে তাদের জানানো।
Method সাধারণত থাকে:
attach(observer) → observer যোগ করা
detach(observer) → observer বাদ দেওয়া
notify() → সবাইকে জানানো


2️⃣ Observer
যারা সেই change/event শুনবে।
Subject তাদেরকে notify করলে, observer তাদের নিজস্ব কাজ করবে।
Method সাধারণত থাকে:
update($message) → Subject থেকে আসা মেসেজ হ্যান্ডেল করা



3️⃣ Concrete Subject & Concrete Observers

Concrete Subject → আসল class, যেখানে আসলে state change হয় (যেমন: Teacher)।
Concrete Observer → আসল class, যারা notify পায় (যেমন: Student)।

### ছোট্ট Flow

Subject event ঘটায় (যেমন: Teacher → “পরীক্ষা হবে”)
Subject → notify() চালায়
Observer-রা update() method দিয়ে মেসেজ পায়


### সহজ PHP উদাহরণ:

```
<?php
// Observer Interface
interface Observer {
    public function update($message);
}

// Subject Class
class Teacher {
    private $observers = [];

    public function attach(Observer $observer) {
        $this->observers[] = $observer;
    }

    public function notify($message) {
        foreach ($this->observers as $observer) {
            $observer->update($message);
        }
    }
}

// Concrete Observers (Students)
class Student implements Observer {
    private $name;

    public function __construct($name) {
        $this->name = $name;
    }

    public function update($message) {
        echo $this->name . " received message: " . $message . "<br>";
    }
}

// ব্যবহার
$teacher = new Teacher();

$student1 = new Student("Rasel");
$student2 = new Student("Rahim");

$teacher->attach($student1);
$teacher->attach($student2);

// শিক্ষক সবাইকে জানালেন
$teacher->notify("আগামীকাল পরীক্ষা হবে!");
```

### Output

```
Rasel received message: আগামীকাল পরীক্ষা হবে!
Rahim received message: আগামীকাল পরীক্ষা হবে!
```




















