## Class 3: Passing Functions as Props


#### This topic matters as it relates to what I am studying in this module because...
Lab 03 requires updating state using the child's props in several different instances. 


## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

#### What does .map() return?
    A new Array

#### If I want to loop through an array and display each value in JSX, how do I do that in React?
By running your array through .map and returning a li. 
ie:
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>


#### Each list item needs a unique ____.
    Key

#### What is the purpose of a key?
    "Keys help React identify which items have changed, are added, or are removed."

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

#### What is the spread operator?
"a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments."

the ... "spread syntax “spreads” the array into separate arguments."

#### List 4 things that the spread operator can do.
    * Copying an array
    * Concatenating or combining arrays
        * Using Math functions
        * Using an array as arguments
        * Adding an item to a list
        * Adding to state in React
        * Combining objects
        * Converting NodeList to an array


#### Give an example of using the spread operator to combine two arrays.
const myArray = [1, 2, 3, 4]
const yourArray = [5, 6, 7, 8]
const ourArry = [...myArray, ...yourArray]
console.log (...ourArray)//12345678

#### Give an example of using the spread operator to add a new item to an array.
const number = [1, 2, 3, 4, 5]
const moreNumbers= [0, ...number]
console.log (moreNumbers);

#### Give an example of using the spread operator to combine two objects into one.

let objectOne = {hello: 1}
let objectTwo = {world: 2}
let objectThree = {...objectOne, ...objectTwo, laugh: 3}
console.log(objectThree);

## Videos

### [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

#### In the video, what is the first step that the developer does to pass functions between components?
by create the function wherever the state is that we are going to change.


#### In your own words, what does the increment function do?
It increases the count of the person passed in using the setState function.

#### How can you pass a method from a parent component into a child component?
By using prop

#### How does the child component invoke a method that was passed to it from a parent component?
 by using the prop to invoke it. 

### Bookmark and Review

* React Tutorial through ‘Declaring a Winner’

* React Docs - Lifting State Up