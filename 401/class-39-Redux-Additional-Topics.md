# Redux - Additional Topics


## Reading

### [Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)

#### What concerns are addressed by Redux Toolkit?

Redux Toolkit addresses concerns such as boilerplate code, complex setup, and repetitive tasks involved in setting up a Redux store. It provides a simplified and opinionated approach to configuring Redux, including standardized ways to define actions, reducers, and store setup.

#### What does `configureStore()` do?

`configureStore()` is a function provided by Redux Toolkit that combines several Redux store setup steps into one. It sets up the Redux store with sensible defaults, including the Redux DevTools extension integration and enables additional middleware like Redux Thunk or Redux Saga.

#### How would I use `createSlice()`?

`createSlice()` is a function from Redux Toolkit that simplifies the process of creating Redux reducers and actions. It takes an initial state, a collection of reducer functions, and generates a slice of the Redux state with corresponding action creators and reducer logic, reducing the amount of boilerplate code needed.

### [MobX](https://mobx.js.org/getting-started.html)

#### What is Mobx?

MobX is a state management library for JavaScript applications. It provides a simple and reactive way to manage application state, where changes to the state are automatically tracked, and the affected parts of the user interface are updated accordingly.

#### How does MobX make it “impossible” to produce an inconsistent state?

MobX achieves consistency by enforcing strict rules for modifying the state. It only allows state modifications to happen within MobX-tracked functions, known as "actions." By ensuring that state changes are made through actions, MobX can track dependencies accurately and update the user interface consistently.

#### How would we build a reactive user interface?

To build a reactive user interface with MobX, you would define observable state variables using MobX decorators or observable() function. Then, you would create computed values that derive from the state, and MobX will automatically track their dependencies. Finally, you bind the reactive values to the UI components, and they will be automatically updated whenever the state changes.

### [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

#### What take-away(s) did this tutorial provide?

The [Redux Toolkit Quick Start tutorial](https://redux-toolkit.js.org/tutorials/quick-start) briefly shows how to add and use Redux Toolkit in a React application.

The [Redux Essentials tutorial](https://redux.js.org/tutorials/essentials/part-1-overview-concepts) teaches you "how to use Redux the right way", using Redux Toolkit as the standard approach for writing Redux logic.

The [Redux Fundamentals tutorial](https://redux.js.org/tutorials/fundamentals/part-1-overview) teaches "how Redux works, from the bottom up", by showing how to write Redux code by hand and why standard usage patterns exist. It then shows how Redux Toolkit simplifies those Redux usage patterns.

### Bookmark and Review

#### [Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

#### [HookState](https://hookstate.js.org/)


### Reflection

What are your learning goals after reading and reviewing the [class README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-39/)?

I want to learn to better manage state utilizing Redux. 