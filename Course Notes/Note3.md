# Section 4
### NULL
- null constant
```php
$x =null;
```
- undefined variables
to check value is null or not:
- is_null()
- null === $x
#### excplicitly unset
```php
$x = 123;
unset($x); //null
```
----------------------------------------

### Arrays
to define an array:
```php
// 1
$arr =['x','y','z'];
// 2
$arr = array('a','b');

```
- you can not access using negative numbers "you will get a warning"
- to check if the item exist in this index or not try {isset($arr[5])}

#### Print array 
```php
print_r($arr);
echo '<pre>';
print_r($arr);
echo '</pre>' ;
```
- push elements in array
```php
$arr[] = 123;
array_push($arr,1,2,3);
```
#### Associative array 
you specify the key and the value
- `note` :values can be another array and it called multi dim array.
```php
$arr ={
    'php' => '8.0'
    , 'python' => '3.9'
}

```
- to access it use the key.
- if there is multi key use the form { $arr['key1']['key2']..}
- keys should be string or int because PHP cast it when possible and the last one will override.
- null keys are casted into empty string
- keys icremented as 0, 1, 50, 51, 52
- pop elements from array
```php
//1
array_pop($arr); //retern last elrm
//2
array_shift($arr); // return first elem and re-indxe the array if the keys is nums
//3
unset($array[1]); //remove specific elem
```
- `note` if you unset the entire elems it will be setted to null so when you try to push you will get the next empty.

- array_key_exists() to check if the key exist
- isset() false if null 
