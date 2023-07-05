# Redux - Asynchronous Actions

## [async actions](https://redux.js.org/advanced/asyncactions)

### Why use Redux middleware?

Redux middleware is used to extend the functionality of Redux by intercepting actions before they reach the reducers. It enables handling of asynchronous operations, logging, API calls, and more, by providing a way to modify actions or dispatch additional actions.

### Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

In the Redux Async Data Flow Diagram, an action is dispatched to trigger an asynchronous operation. The middleware intercepts the action and can perform tasks like API calls. Once the async operation completes, it dispatches a success or failure action. The reducer updates the state based on the received action.

### How are we accommodating async in our Redux app?

Async operations in Redux can be accommodated by using middleware like Redux Thunk or Redux Saga. Redux Thunk allows writing action creators that return functions instead of plain action objects. These functions can contain asynchronous logic, such as API requests, and dispatch further actions based on the async results.


## [thunk middleware](https://github.com/reduxjs/redux-thunk)

### Why would you need redux-thunk middleware?

Redux Thunk middleware is useful when dealing with asynchronous operations in Redux. It allows action creators to return functions instead of plain actions, enabling them to dispatch multiple actions, delay dispatching, or perform conditional dispatching based on async results.

### Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

Redux Thunk middleware allows action creators to return a function instead of an action. This function is known as a thunk. Thunks can be used to encapsulate asynchronous logic and dispatch actions based on the async results.

### Describe how any return value from the inner thunk function will be made available.

The return value from the inner thunk function will be made available through the dispatch function. When the inner thunk function is executed, it can dispatch multiple actions, including success or failure actions. These actions can be handled by the reducers to update the state accordingly.


## Reflection

### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-38/)?

To dive deeper into my understanding of the thunk redux middleware and its utilization. 