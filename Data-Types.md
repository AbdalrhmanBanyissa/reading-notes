# Java Data Types
As explained in the previous chapter, a variable in Java must be a specified data type:

#### Example
```java
int myNum = 5;               // Integer (whole number)
float myFloatNum = 5.99f;    // Floating point number
char myLetter = 'D';         // Character
boolean myBool = true;       // Boolean
String myText = "Hello";     // String
```

Data types are divided into two groups:

* Primitive data types - includes `byte`, `short`, `int`, `long`, `float`, `double`, `boolean` and `char`
* Non-primitive data types - such as String, Arrays and Classes (you will learn more about these in a later chapter)

## Primitive Data Types
A primitive data type specifies the size and type of variable values, and it has no additional methods.

There are eight primitive data types in Java:


| Data Type | Size | Description     |
| ----------|------|-----------------|
|byte|1 byte|Stores whole numbers from -128 to 127|
|short|2 byte|Stores whole numbers from -32K to 32K|
|int|4 byte|Stores whole numbers from -2B to 2B|
|long|8 byte| |
|float|4 byte||
|double|8 byte||
|boolean|1 byte|Stores true or false values|
|char|2 byte|	Stores a single character|

## Non-Primitive Data Types
Non-primitive data types are called **reference types** because they refer to objects.

The main difference between **primitive** and **non-primitive** data types are:

* Primitive types are predefined (already defined) in Java.
Non-primitive types are created by the programmer and is not defined by Java (except for `String`).
* Non-primitive types can be used to call methods to perform certain operations, while primitive types cannot.
* A primitive type has always a value, while non-primitive types can be `null`.
* A primitive type starts with a lowercase letter, while non-primitive types starts with an uppercase letter.
* The size of a primitive type depends on the data type, while non-primitive types have all the same size.