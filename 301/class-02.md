[React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
Render

### What is the very first thing to happen in the lifecycle of React?
Mounting constructor

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
   * constructor
   * Render
   * React updates
   * componentDidMount
   * componentWillUnmount



### What does componentDidMount do?
"This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount()."


## Videos
[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

* What types of things can you pass in the props?
props are arguements you pass inside a function. If you have a component inside of react and you want to render it you're going to pass is the props you want to give to it.
Props is for things that you passed. It's like a function there what you want to initialize your component to or what you want your component to render. 
If you want to display something to the user that has a title and subtitle. 

* What is the big difference between props and state?
state is something inside of a component.
Props: You pass into a component. Props are handled outside of the component.
Props are useful when you want to display some information inside of a component. 
State: is handled inside of that component.
Helpful when we are going to be changing or updatine something 9(ie, a counter)


* When do we re-render our application?
when you change the state inside of your application. 

* What are some examples of things that we could store in state?
form information
updating a counter

## Bookmark and Review
React Docs - State and Lifecycle
React Docs - handling events
React Tutorial through ‘Developer Tools’
React Bootstrap Documentation
Boootstrap Cheatsheet
Bootstrap Shuffle - a class “sandbox”
Netlify