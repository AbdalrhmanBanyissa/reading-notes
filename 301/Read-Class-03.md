# Passing Functions as Props

## React Docs - lists and keys

What does .map() return?

* it returnes an array with lenght is equal to the original (maped) array.

If I want to loop through an array and display each value in JSX, how do I do that in React?

* By using the JavaScript map() function.

Each list item needs a unique ____.

* < li > tag

What is the purpose of a key?

* Keys help React identify which items have changed, are added, or are removed.

## The Spread Operator

What is the spread operator?

* spread syntax refers to the use of an ellipsis of three dots (β¦) to expand an iterable object into the list of arguments.

List 4 things that the spread operator can do.

* Take trying to find the largest number in an array with Math.max()

* Trying to pass an array to a JavaScript function expecting separate arguments does not work. In this case it produces a NaN result. Enter β¦

* The spread syntax βspreadsβ the array into separate arguments.

* Converting NodeList to an array

Give an example of using the spread operator to combine two arrays.

```javascript
const fruits = ['π','π','π','π','π']

const moreFruits = [...fruits];

console.log(moreFruits) // Array(5) [ "π", "π", "π", "π", "π" ]

fruits[0] = 'π'

console.log(...[...fruits,'...',...moreFruits]) // π π π π π ... π π π π π
```

Give an example of using the spread operator to add a new item to an array.

```javascript
const fewFruit = ['π','π','π']
const fewMoreFruit = ['π', 'π', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "π", "π", "π", "π", "π" ]
```

Give an example of using the spread operator to combine two objects into one.

```javascript
[...["ππππ€ͺπ"]] // Array [ "ππππ€ͺπ" ]
[..."ππππππ₯°ππ€©!"] // Array(9) [ "π", "π", "π", "π", "π", "π₯°", "π", "π€©", "!" ]

const hello = {hello: "ππππ€ͺπ"}
const world = {world: "ππππππ₯°ππ€©!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "ππππ€ͺπ", world: "ππππππ₯°ππ€©!" }
```

## How to Pass Functions Between Components

In the video, what is the first step that the developer does to pass functions between components?

* It should increment and pass the object from the function, then use the map function

In your own words, what does the increment function do?

* It helps us to know what is the next node in the same level. From there it increases the level of that node by one in A of that level.

How can you pass a method from a parent component into a child component?

* First we define our parent callback function in the parent component, then we pass the function to the child component, after that we set up an input variable in the child component and the last thing is the callback function.

How does the child component invoke a method that was passed to it from a parent component?

* Using the 'this' method that calls the method passed to it from the main component.