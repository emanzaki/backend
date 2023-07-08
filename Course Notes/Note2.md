# Section 3
### numbers 
you can't trust comparing numbers in PHP 
ex:
```php
$x=0.23;
$y=1-0.77;
# x , y are not equal even both are float and have the same value
echo (bool)($x==$y); //print empty string meaning false
```
because it depends on how float numbers stored in binary in the memory.
- NAN = log(-1)
- INF "out of range"
- is_infinite() or is_finite()
- is_nan()

-----------------------------------
### strings 
diff between '' and "" is
'' -->> can't be used for var
"" -->> can be used 
- use {} for a better readability
- to access a specific letter use 0,1,2  
from the beginning and -1,-2,-3 from the back
- it keeps your white spaces but not when you print it 
```php
<?php
$x="    ioj";
var_dump($x);
?>
```
#### Heredoc
u can use variables
```php
$text =<<<TEXT
al;mfcalmfs
ldm;ldv
;ladm
TEXT;
```
#### Nowdoc
```php
$text=<<<'TEXT'
dkmvksmd
s;ldmvl;md
ldmal;f
TEXT;
```

- heredoc and nowdoc can be used without escape charcters for " or ' and you can have a full html inside.
