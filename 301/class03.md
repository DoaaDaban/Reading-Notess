#  Passing Functions as Props

## Lists and Keys

const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);


## Rendering Multiple Components

const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

## Basic List Component

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);

## React Docs - lists and keys ..
**What does .map() return ?**
- return new array with modified data .
**If I want to loop through an array and display each value in JSX, how do I do that in React ?**
- You can build collections of elements and include them in JSX using curly braces {}.
-  we loop through the elements array using the JavaScript map() function.
**Each list item needs a unique ____.**
- Key .
**What is the purpose of a key ?**
- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.
## The Spread Operator ..
**What is the spread operator?**
- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function's arguments.
**List 4 things that the spread operator can do.**
- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
**Give an example of using the spread operator to combine two arrays.**
- using the … spread operator is a convenient way to copy an array or combine arrays, and it can even add new items.
> const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
**Give an example of using the spread operator to add a new item to an array.**
- the spread operator can add an item to an another array with a natural, easy-to-understand syntax.
> const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
**Give an example of using the spread operator to combine two objects into one.**
- he spread syntax is useful for combining the properties and methods on objects into a new object.
> const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂