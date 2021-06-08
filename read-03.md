# Read 03: Passing Functions as Props:

## React Docs - lists and keys:

**map() return an new array with changes but with the same length.**

const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);

**We can loop through an array and display each value in JSX by using the .map() array method.**

**Each list item needs a unique Key.**

**What is the purpose of a key?**
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

--------------------------------------------------------------------

## The Spread Operator:

**What is the spread operator?**
JavaScript's spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

**The spread operator can do: Copying an array, Concatenating or combining arrays, Using Math functions & Using an array as argument.**

//ex
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

//ex
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

//ex
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

## Passing Functions between Components:

**In the video, what is the first step that the developer does to pass functions between components?**
Create a function in the parent component.

**In your own words, what does the increment function do?**
It increments the count variablie which was also passed from the parent to the child by one.

**How can you pass a method from a parent component into a child component?**
By sending it as a prop, and in the child component you can call inside another function.

**How does the child component invoke a method that was passed to it from a parent component?**
It invokes the method inside a method written inside of it, and if a parameter was a passed prop, you can call it using this.props.nameofprop as an argument.

---------------------------------------------------------------------

### Things I want to know more about:
- Know more about the spread opartors and how to use them effeciently.
