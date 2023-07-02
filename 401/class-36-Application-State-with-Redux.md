## Application State with Redux


### Reading

[Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

* What is the first principle of Redux?

The first principle of Redux is that the entire application state is stored in a single JavaScript object called the "store."

* what is a store and what do we use our reducers for within that store?

The store in Redux is an object that holds the application state and provides methods for accessing and updating it. Reducers are functions used within the store to handle specific actions and update the state accordingly.

* Name three Redux store methods given to us by createStore and describe their use.

Three Redux store methods provided by createStore are:

`getState()`: Retrieves the current state from the store.
`dispatch(action)`: Dispatches an action to trigger a state change.
`subscribe(listener)`: Registers a listener function that is called whenever the state changes.


* Explain to a non-technical recruiter what combineReducers() does and why it is useful.

combineReducers() is a Redux function used to combine multiple reducers into a single reducer function. It helps manage different parts of the application state by assigning each reducer to a specific key in the overall state object. This modular approach improves code organization, reusability, and maintainability in complex applications.

### Bookmark and Review

[worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)

### Additional Questions

#### Looking ahead at this module’s [course schedule](https://codefellows.github.io/code-401-javascript-guide/curriculum/#module-8), What do you look forward to learning?

I know redux is very useful in React, so I look forward to learning more about it. 

#### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-36/)?

Learning to manage state with Redux