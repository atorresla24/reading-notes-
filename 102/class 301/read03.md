# reading 03

## React Docs - lists and keys

1. .map() returns a new array
2. If you want to loop through an array and display each value of JSX by returning an <li> element for each item.
3. Each list item needs a unique key
4. The purpose of a key is to help React identify which items have changed, are added, or are removed

## The Spread operator

1. The spread operator refers to the use of an ellipsis of three dots to expand an iterable object into the list of arguments.
2. The spread operator can: copy an array, concatenating or combining arrays, use math functions, use an array as arguments.
3. An example of using the spread operator to combine two arrays: 
const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ
4. An example of using the spread operator to add a new item to an array:
const fewFruit = ['ð','ð','ð']
const fewMoreFruit = ['ð', 'ð', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]
5. An example of using the spread operator to combine two objects into one:
const objectOne = {hello: "ðĪŠ"}
const objectTwo = {world: "ðŧ"}
const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("ð".repeat(5))}}
objectFour.laugh() // ððððð

## How to pass functions between components

1. The first step that the developer does to pass functions between components is create a function wherever the state is.
2. The increment function loops through the array until it finds the name of the person and adds +1 to the count of the person.
3. A method can be passed from a parent component into a child component by using this.props...
4. The child component invokes a method that was passed to it from a parent component by using this.props.'method name'(this.props.'parent component property').

## Things I want to know more about

I want to be able to understand more about how the spread operator can be used in different situations

