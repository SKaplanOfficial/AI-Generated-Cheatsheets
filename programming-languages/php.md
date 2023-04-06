# PHP Cheatsheet

PHP is a server-side scripting language used for web development. It provides features such as dynamic typing, arrays, functions, loops, conditionals, and file manipulation to help developers build dynamic and interactive web applications. This cheatsheet provides an overview of some of the key features of PHP, along with code blocks for variables, functions, loops, conditionals, file manipulation, and resources for further learning.

## Variables

```php
// Declaring a variable
$myString = 'Hello, World!';
$myNumber = 42;
$myBoolean = true;

// Concatenating strings
$fullName = $firstName . ' ' . $lastName;

// Variable scope
function myFunction() {
  global $myVariable; // Accessing a global variable
  $localVariable = 'Local variable'; // Declaring a local variable
}
```

## Functions

```php
// Declaring a function
function addNumbers($a, $b) {
  return $a + $b;
}

// Declaring a function with default parameters
function sayHello($name = 'World') {
  echo 'Hello, ' . $name . '!';
}

// Declaring a function with variable arguments
function sum(...$numbers) {
  return array_sum($numbers);
}

// Declaring an anonymous function
$myFunction = function($param) {
  // function body
};
```

## Loops

```php
// for loop
for ($i = 0; $i < 10; $i++) {
  echo $i;
}

// foreach loop
$myArray = array(1, 2, 3, 4, 5);
foreach ($myArray as $item) {
  echo $item;
}

// while loop
$i = 0;
while ($i < 10) {
  echo $i;
  $i++;
}

// do...while loop
$j = 0;
do {
  echo $j;
  $j++;
} while ($j < 10);
```

## Conditionals

```php
// if statement
if ($myNumber === 42) {
  echo 'The answer to the ultimate question of life, the universe, and everything';
}

// if...else statement
if ($myBoolean) {
  echo 'The boolean is true';
} else {
  echo 'The boolean is false';
}

// ternary operator
$result = $myNumber > 0 ? 'Positive' : 'Negative or zero';

// switch statement
switch ($myString) {
  case 'Hello':
    echo 'The string is "Hello"';
    break;
  case 'World':
    echo 'The string is "World"';
    break;
  default:
    echo 'The string is something else';
    break;
}
```

## File manipulation

```php
// Including a file
include 'myfile.php';

// Requiring a file
require 'myfile.php';

// Reading a file
$myfile = fopen('myfile.txt', 'r');
echo fread($myfile, filesize('myfile.txt'));
fclose($myfile);

// Writing to a file
$myfile = fopen('myfile.txt', 'w');
fwrite($myfile, 'Hello, World!');
fclose($myfile);
```

## Resources

- [PHP documentation](https://www.php.net/manual/en/index.php)
- [PHP tutorial](https://www.w3schools.com/php/)
- [PHP with MySQL tutorial](https://www.w3schools.com/php/php_mysql_intro.asp)
- [Laravel framework](https://laravel.com/)
- [Symfony framework](https://symfony.com/)