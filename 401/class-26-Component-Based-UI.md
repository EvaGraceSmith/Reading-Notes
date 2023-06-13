## Component Based UI

### [React Quick Start](https://react.dev/learn)



#### What are the building blocks of a React app?

"The building blocks of a React app are components. Components are reusable, self-contained units that encapsulate the UI and its logic.

#### What is the difference between an HTML element and a React component?

An HTML element is a predefined tag that represents an element on a webpage, while a React component is a reusable piece of UI logic that can be composed to create complex UIs.

#### What is JSX and why do we use it?

JSX is a syntax extension for JavaScript that allows you to write HTML-like code within JavaScript. It is used in React to define the structure and appearance of UI components.

#### Describe the process of embedding JavaScript expressions in JSX.

JavaScript expressions can be embedded in JSX by wrapping them within curly braces {}. For example, `<div>{2 + 2}</div>` would render as `<div>4</div>`.

#### Does React or JSX have any special features for iteration or conditional logic?

React has special features like mapping and conditional rendering for iteration and conditional logic. JSX allows you to use JavaScript expressions and control structures within curly braces to conditionally render components or iterate over arrays.

#### How does React know to respond to a user’s inputs?

React responds to user inputs through event handling. Components can listen for events like onClick or onChange and update their state accordingly, triggering re-rendering of the affected parts of the UI.

#### What word indicates that a React component manages data with a Hook?

The word that indicates a React component manages data with a Hook is "useState". Hooks are functions that allow functional components to manage state and perform other React-related tasks.
#### How can two react components share data?

Two React components can share data by lifting the state up to a common ancestor component and passing it down as props. The child components can then access and update the shared data through the props.
### [Render and Commit](https://react.dev/learn/render-and-commit)


#### What are the three steps of refreshing a React UI?

The three steps of refreshing a React UI are rendering, reconciliation, and committing. Rendering calculates the new UI representation, reconciliation determines the changes, and committing updates the DOM with the changes.

#### How do you trigger updates to a component after the initial render?

Updates to a component after the initial render can be triggered by changing the component's state using setState() or by receiving new props from its parent component.
#### Does React recreate DOM nodes on every rerender?

No, React does not recreate DOM nodes on every rerender. It uses a virtual DOM and performs a diffing algorithm to determine the minimal set of changes needed to update the actual DOM efficiently.

#### After React has updated the DOM, what still needs to happen before the user sees the change?

After React has updated the DOM, the browser still needs to paint the changes on the screen. This process is called layout and painting, and it involves the browser calculating the positions and styles of the updated elements and rendering them visually.

### Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

[Your First Component](https://react.dev/learn/your-first-component)

[Importing and Exporting Components](https://react.dev/learn/importing-and-exporting-components)

[Writing Markup with JSX](https://react.dev/learn/writing-markup-with-jsx)

[sass cheatsheet](https://devhints.io/sass)

[react cheatsheet](https://devhints.io/react)


### Additional Questions

Note the naming conventions in the [Airbnb React/JSX Style Guide](https://airbnb.io/javascript/react/#naming). What pattern(s) do you see?

File Names: Files containing React components are typically named using PascalCase, where the file name matches the name of the component. For example, a component named MyComponent would be defined in a file called MyComponent.js.

Component Names: React component names are also written in PascalCase. This helps differentiate them from regular HTML elements. For example, a component might be named MyComponent.

Props: Props passed to components are usually named using camelCase. For example, a prop for a component could be named myProp.

State Variables: State variables in React components are often prefixed with the word "is" or "has" to indicate that they represent a boolean value. For example, a state variable indicating whether a component is active could be named isActive.

Event Handlers: Event handler functions are typically named using the "handle" prefix followed by the event and the action. For example, a function handling a click event could be named handleClick.

Private Methods: Private methods, which are internal to a component and not meant to be accessed externally, are often prefixed with an underscore. For example, a private method could be named _calculateTotal.' - ChatGPT

#### Looking ahead at this module’s course schedule, What do you look forward to learning?

I am looking forward to getting back to good ol' React and sinking my teeth into hooks

#### What are your learning goals after reading and reviewing the class README?


I am excited to learn SASS!!