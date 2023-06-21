## Reading: useState() Hook


## Reading

### [Thinking in React](https://react.dev/learn/thinking-in-react)

#### Summarize the five steps of thinking in react.

1. Break the UI into a component hierarchy: Analyze the user interface and identify the major components and their relationships. Divide the UI into smaller, reusable components.

2. Build a static version: Create a static version of the UI with hard-coded data and no interactivity. Focus on building the components and their structure.

3. Identify the minimal (but complete) representation of UI state: Determine the minimal set of state that is needed for the UI to be rendered correctly and update as necessary. This involves identifying which components should manage which state.

4. Identify where the state should live: Determine which component or components should own and manage the identified state. Choose the component that is higher up in the component hierarchy and is shared by the components that need access to the state.

5. Add inverse data flow: Establish the flow of data and interactivity by adding event handlers and callbacks. Update the state when necessary and propagate the changes to the appropriate components. Ensure that the UI reflects the updated state and responds to user interactions.

### [State: A Component’s Memory](https://react.dev/learn/state-a-components-memory)

### What is one reason a local variable isn’t sufficient for managing a React component?

One reason a local variable isn't sufficient for managing a React component is that local variables don't persist their values between re-renders, causing the loss of component state.


### What is the argument to the useState hook, and what are the two parts of its return array?

The argument to the useState hook is the initial state value. The two parts of its return array are the current state value and a function to update the state.

### How can Component A access state from Component B?

Component A can access state from Component B by either lifting the state up to a common ancestor component and passing it as props to both components, or by using a state management library like Redux or React Context.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

[Passing Props to a Component](https://react.dev/learn/passing-props-to-a-component)

[Rendering Lists](https://react.dev/learn/rendering-lists)

[State as Snapshot](https://react.dev/learn/state-as-a-snapshot)

[useState hook](https://react.dev/reference/react/useState)

## Reflection

### What are your learning goals after reading and reviewing the class README?

I am looking forward to diving deeper into hooks!