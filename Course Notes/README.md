# Section 1:
what is a web server?
---------------------------
### What is the alt for installing PHP to OS?
- VM / Docker
- XAMPP / MAMP
--------------------------------------
### working with xampp:
- to get the source code running go to hdocs and install your own files.
---------------------------------------
- Parse error if you forget the semi-colon ';'
- executing PHP in cmd
```bash
 php index.php
```
- ',' and '.' both work for concatenation in "echo" 
- can not assign $this will get a fatal error because it's an object
- if you want to execute PHP code should have the tag <?PHP ?>
## comments 
- // /* */ 
- can not comment end ?> tag
-----------------------------------------
# section 2:
getting started with PHP.
### constants
- usual constants
```php
#by func
define('name','eman'); //runtime
#const keyword
const x =10; //compile time
```
- dynamic constants
```php
$x=50;
define('num'.$x,$x);
```
- pre-defined constants: PHP_VERSION..etc
- magical constants: __ LINE__..etc
-------------------------------
### variables 
- you can assign a variable with 
```php
#ref :
    $y= &$x
#value : 
    $y=$x
```
- variable variables:+
```php 
$foo ='bar';
$$foo ='baz';

echo $bar;
```
------------------------------------
### Types
> To get the type of any data use getttype() func.
#### Scalar Types
- bool
- int
- float
- string 
```php 
$x= true;
$y= 20;
$z=0.2;
$name='eman';
```
#### Compound Types
- array 
- object
- callable
- iterable
```php
$arr=[1,2,3,4] #can be mixed types 
#to print any array use print_r(arr);
```
#### Special Types
- resource
- null
------------------------------
### Type hinting 
 It's when you define the type you want to get. 
example :
```php 
function sum (int $x,int $y){
    return $x + $y;
}
``` 
 so if you pass a string or float it will be cast into an integer otherwise will throw a fatal error
 - you can also use a strict mode to just get the integer you want 
 ```php 
declare(strict_types=1);
```
