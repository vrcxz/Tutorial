Declaring class:
```php
class ClassName{
//code
}
```


Creating an object:
```php
$variablename = new ClassName();
```


Inheriting a class:
```php
class ClassName1 extends ClassName2{
//code
}
```

Inheriting is basically just like copy/pasting everything inside the class to the other class.


How to call a variable or a function inside a class:
```php
$this->variablename();
$this->functionname();
```

Access modifiers:
public - you can call a variable/function anywhere (outside the class, inside the class, inside the inherited class)

protected - you can call a variable/function inside the class, and inside the inherited class. You will get error if you try to call outside of the class.

private - you can call a variable/function inside the class only. You will get an error if you try to call outside of the class or in the inherited classes.


How to access private variables:
Use set and get functions.

Example:
```php
class Fruit{
 private $name;
}

$apple = new Fruit();
$apple->name = 'Star Apple'; //Will give an error because it's private
echo $apple->name; //Will also give an error because it's private
```

It should be:
```php
class Fruit{
 private $name;

 function set($value){
  $this->name;
 }

 function get(){
  return $this->name;
 }
}

$apple = new Fruit();
$apple->set('Star Apple');
echo $apple->get(); //Will work
```
