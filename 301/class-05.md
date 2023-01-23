## Class 05- React




#### How does this subject matter as it relates to what I am studying?
We are currently working in react



Reading
[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

### What is the single responsibility principle and how does it apply to components?
* "a component should ideally only do one thing.If it ends up growing, it should be decomposed into smaller subcomponents."

### What does it mean to build a ‘static’ version of your application?
* It means to build a version that takes your data model and renders the UI but has no interactivity.
* Building a static version requires a lot of typing and not thinking. (Whereas adding interactivity requires a lot of thinking and not a lot of typing.)

### Once you have a static application, what do you need to add?
* interactivity

### What are the three questions you can ask to determine if something is state?
* Is it passed in from a parent via props? If so, it probably isn’t state.
* Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.

### How can you identify where state needs to live?

* Identify every component that renders something based on that state.
* Find a common owner component (a single component above all the components that need the state in the hierarchy).
* Either the common owner or another component higher up in the hierarchy should own the state.
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.



### [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)


### What is a “higher-order function”?
* "Functions that operate on other functions, either by taking them as arguments or by returning them"



### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

* Creating a condition of returning m if m is greater than n

### Explain how either map or reduce operates, with regards to higher-order functions.
* "The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function."
* 


#### Things I want to know more about:
I would like to review my beast data code and see if I can figure out how to better organize it after reading the first article.
The second is very useful for the code challenge, and I look forward to comparing the information here with a couple of the challenges I was stuck on to see if I can get further. 