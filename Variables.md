# Java Variables

## Java Variables
Variables are containers for storing data values.

In Java, there are different **types** of variables, for example:

* `String` - stores text, such as "Hello". String values are surrounded by double quotes
* `int` - stores integers (whole numbers), without decimals, such as 123 or -123
* `float` - stores floating point numbers, with decimals, such as 19.99 or -19.99
* `char` - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
* `boolean` - stores values with two states: true or false

## Declaring (Creating) Variables
To create a variable, you must specify the type and assign it a value:
#### Syntax
```java
type variable = value;
```
Where *type* is one of Java's types (such as `int` or `String`), and variable is the name of the variable (such as **x** or **name**). The **equal sign** is used to assign values to the variable.

#### Example
Create a variable called **name** of type `String` and assign it the value "**John**":
```java
String name = "John";
System.out.println(name);
```

## Final Variables
However, you can add the `final` keyword if you don't want others (or yourself) to overwrite existing values (this will declare the variable as "final" or "constant", which means unchangeable and read-only):
#### Example
```java
final int myNum = 15;
myNum = 20;  // will generate an error: cannot assign a value to a final variable
```

