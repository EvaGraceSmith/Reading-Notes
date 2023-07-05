## Redux - Combined Reducers



### [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

1. Why create multiple reducers?

Multiple reducers are created to handle different slices of state in a Redux application, making the code more organized and maintainable.

2. How would you combine multiple reducers

To combine multiple reducers, you use Redux's combineReducers function, providing an object mapping the individual reducers to their corresponding state slices.

3. How will you manage state as an immutable object? why?

State is managed as an immutable object in Redux to ensure predictability, traceability, and easy debugging. Immutable state prevents direct mutations, helping to avoid unintended side effects and simplifying state change tracking through the use of pure functions.

### Redux Docs: Using Combined Reducers

1. combineReducers is a utility function to simplify the most common use case when writing ___ _____ .

 Redux reducers with multiple "slice reducers" managing different parts of the state.

2. Explain how combineReducers assembles the new state tree.

combineReducers assembles the new state tree by calling each slice reducer with its current slice of state and the current action. It combines the individual slice updates into a new state object.

3. How would you define initial state in an app using combineReducers?

Initial state in an app using combineReducers can be defined in two ways:

* The createStore function can take preloadedState as its second argument.
* The root reducer can return the initial state value when the state argument is undefined.


### [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

1. Why will you want to split your reducing functions as your app becomes more complex?

Splitting reducing functions becomes necessary as the app becomes more complex to manage different parts of the state separately. It improves modularity, maintainability, and allows multiple reducers to independently handle specific data domains or features.


2. The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.


The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to the Redux store.

3. What is a popular convention when naming reducers?

A popular convention when naming reducers is to use descriptive names that reflect the domain or type of data they handle. It is generally not recommended to include words like "reducer" in the reducer's name, as the keys in the state object should simply reflect the nature of the data they hold.

### Reflection

#### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-37/)?

I am hoping to dive deeper into my understanding of Redux