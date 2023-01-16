
## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

* What does .map() return?
    A new Array
* If I want to loop through an array and display each value in JSX, how do I do that in React?

* Each list item needs a unique ____.
    Key
* What is the purpose of a key?
    "Keys help React identify which items have changed, are added, or are removed."

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

* What is the spread operator?
"a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments."

the ... "spread syntax “spreads” the array into separate arguments."

* List 4 things that the spread operator can do.
    * Copying an array
    * Concatenating or combining arrays
        * Using Math functions
        * Using an array as arguments
        * Adding an item to a list
        * Adding to state in React
        * Combining objects
        * Converting NodeList to an array


* Give an example of using the spread operator to combine two arrays.
const myArray = [1, 2, 3, 4]
const yourArray = [5, 6, 7, 8]
const ourArry = [...myArray, ...yourArray]
console.log (...ourArray)//12345678

* Give an example of using the spread operator to add a new item to an array.
const number = [1, 2, 3, 4, 5]
const moreNumbers= [0, ...number]
console.log (moreNumbers);

* Give an example of using the spread operator to combine two objects into one.

let objectOne = {hello: 1}
let objectTwo = {world: 2}
let objectThree = {...objectOne, ...objectTwo, laugh: 3}
console.log(objectThree);

## Videos

### [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

* In the video, what is the first step that the developer does to pass functions between components?
by create the function wherever the state is 
* In your own words, what does the increment function do?
increasing the number of
* How can you pass a method from a parent component into a child component?
By using the increment method to update local State

* How does the child component invoke a method that was passed to it from a parent component?
 by using dot increment

### Bookmark and Review

* React Tutorial through ‘Declaring a Winner’

* React Docs - Lifting State Up