## Advanced State with Reducers

### [Extracting State Logic into a Reducer](https://react.dev/learn/extracting-state-logic-into-a-reducer)

#### What is the motivation for adding a reducer?

Alright, let's talk about reducers! You know, sometimes life gets complicated, and managing state in your components becomes a spaghetti bowl of confusion. That's when reducers come to the rescue! They give you a single source of truth and a clear way to update state, making your code easier to follow than a recipe for microwave popcorn.

#### What are actions in the context of a reducer? How are they different than setting state directly?

Actions, my friend, are like secret agents assigned to modify your state. They're little JavaScript objects that tell the reducer what needs to be done. Unlike setting state directly where you're like, "Hey state, take this new value," actions bring structure and intention to the game. They come with a type, payload, and sometimes even a cool codename.

#### What common list operation is useReduce named for, and why?

Ah, the common list operation that useReduce is named for is none other than... drumroll, please... reduce itself! It's like the Gandalf of array methods, taking a bunch of elements and magically transforming them into a single value. Just like Gandalf helps the hobbits on their journey, useReduce helps you wrangle your state like a pro.

#### When should you switch from useState to useReducer?

Now, knowing when to switch from useState to useReducer is like knowing when to swap your hoodie for a tuxedo. If your state management starts getting complex, with intricate logic and interdependent values, it's time to go full-on reducer mode. When useState feels like a rollercoaster ride and you need a more structured approach, that's when you call in the reducer cavalry.

### Bookmark and Review


[useReducer hook](https://react.dev/reference/react/useReducer)
[Keeping Components Pure](https://react.dev/learn/keeping-components-pure)
[Queueing a Series of State Updates](https://react.dev/learn/queueing-a-series-of-state-updates)

### Reflection

What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-29/)?

Yay! More hooks! Excited to learn about the useReducer!