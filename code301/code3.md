# React Docs - lists and keys

**The map()** method creates a new array with the results of calling a function for every array element. The map() method calls the provided function once for each element in an array, in order. Note: map() does not execute the function for array elements without values.



## What does .map() return?

map() returns a map object, which is an iterator that yields items on demand


 ## JSX

>It is a syntax extension to JavaScript. using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.


## If I want to loop through an array and display each value in JSX, how do I do that in React?

const elements = [] //..some array
const items = []
for (const [index, value] of elements.entries()) {
  items.push(&lt;Element key={index} />)
}


## Each list item needs a unique Key 

React uses the key prop create a relationship between the component and the DOM element. The library uses this relationship to determine whether or not the component should be re-rendered.


## What is the purpose of a key?
 Is an inset on a map that explains the symbols, provides a scale, and usually identifies the type of map projection used.
Spread Operator.


# The Spread Operator

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

## List things that the spread operator can do.

*   Copying an array
*  Concatenating or combining arrays
*    Using Math functions
*    Using an array as arguments
*    Adding an item to a list
*    Adding to state in React
*    Combining objects
*    Converting NodeList to an array


## Examples of using :

Here are a couple basic examples of using … in JavaScript, where I demonstrate copying an array, splitting a string into characters, and combining the properties of two JavaScript objects:


[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

Copying an array

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍




