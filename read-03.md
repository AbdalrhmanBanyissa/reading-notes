# HTML Lists, Control Flow with JS, and the CSS Box Model

## HTML Lists

Lists are used to group together related pieces of information so they are clearly associated with each other and easy to read. In modern web development, lists are workhorse elements, frequently used for navigation as well as general content.

### Types

* unordered list `ul` — used to group a set of related items in no particular order

* ordered list `ol` — used to group a set of related items in a specific order

## Boxes in CSS

In CSS, the term "box model" is used when talking about design and layout.

### Dimensions

You can use CSS to control the dimensions of a box.

### Border, Margin, and Padding

You can also control the borders, margin and padding
for each box with CSS.

### Adittional properties

It is possible to hide elements using the display and
visibility properties.

Block-level boxes can be made into inline boxes, and
inline boxes made into block-level boxes.

Legibility can be improved by controlling the width of
boxes containing text and the leading.

## Basic JavaScript Instructions

>statement

`var x, y, z;    // Statement 1`

`x = 5;          // Statement 2`

>Comments

`// This is a comment`

` /* This is a comment too */ `

>Variables

` var x = 5; `

` let x = 5; `

>Data types

![Data types](https://www.creatingux.com/CIT230/media/images/datatypes.png)

>Rules for naming variables

* Variable names cannot contain spaces.

* Variable names must begin with a letter, an underscore (_) or a dollar sign ($).

* Variable names can only contain letters, numbers, underscores, or dollar signs.

* Variable names are case-sensitive.

* Certain words may not be used as variable names, because they have other meanings within JavaScript.

>Arrays

JavaScript arrays are used to store multiple values in a single variable.

` var cars = ["Saab", "Volvo", "BMW"]; `

# Operators and Loops

## Operators

![JS Operators](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/03/JavaScript-Operators-1200x720.jpg)

### Comparison operators

We use **comparison operators** to evaluating conditions and the result of the compareson operator will be booliean value *(true / false)*. Usually comparison operators return a single value.

#### Basic structure

`score >= Pass`   , Which:

* score: operand
* '>=': operator
* pass: operand

 [comparison operators](https://www.w3schools.com/js/js_comparisons.asp)

### Logical operators

**logical operators** allowes us to use two or more compareson operators together in one sentence and return the final value as a *true or false*.

#### Basic structure

 ` 5<2 && 2>=3 `   , Which:

* 2, 3, and 5 are operands
* && logical operator
* '>=, <' compareson operators

[Logical operators](https://www.w3schools.com/js/js_comparisons.asp)

## Loops

### For loop

**For loop** use the counter as a condition and it has a very specific number of iterations.

#### Basic structure

` for (Statement 1;Statement 2;Statement 3){// code block to be executed} `

```the code block.

* Statement 2 defines the condition for executing the code block.

* Statement 3 is executed (every time) after the code block has been executed.

### While loop

**While Loop** can execute a block of code as long as a specified condition is true.

`while (condition){// code block to be executed}`
