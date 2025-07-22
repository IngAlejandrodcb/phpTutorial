# PHP Code Tutorial

This guide provides a quick introduction to writing PHP scripts and running them
from the command line.

## Prerequisites

* PHP installed (`php` command should be available).
* A text editor to create your PHP files.

## 1. Your First PHP Script

Create a file called `hello.php` with the following content:

```php
<?php
echo "Hello, world!\n";
```

Run the script from the command line:

```bash
php hello.php
```

You should see `Hello, world!` printed to the terminal.

## 2. Variables and Types

Variables in PHP are declared with the `$` symbol. PHP is dynamically typed,
so you do not need to specify a type when creating a variable.

```php
<?php
$name = "Alice";
$age = 30;
$height = 1.75; // meters

echo "$name is $age years old and $height meters tall\n";
```

## 3. Control Structures

PHP supports familiar control structures such as `if`, `foreach` and `while`.

```php
<?php
$numbers = [1, 2, 3, 4, 5];

foreach ($numbers as $n) {
    if ($n % 2 === 0) {
        echo "$n is even\n";
    } else {
        echo "$n is odd\n";
    }
}
```

## 4. Functions

Functions are declared using the `function` keyword. You can return values
from functions just like in other languages.

```php
<?php
function add($a, $b) {
    return $a + $b;
}

$result = add(3, 4);
echo "3 + 4 = $result\n";
```

## 5. Running a Local Web Server

PHP provides a built-in web server for testing scripts. From the directory
containing your PHP files, run:

```bash
php -S localhost:8000
```

You can then open `http://localhost:8000/hello.php` in your browser to view
your script's output via HTTP.

This tutorial only scratches the surface. The [PHP manual](https://www.php.net/manual/en/)
offers more extensive documentation and examples.
