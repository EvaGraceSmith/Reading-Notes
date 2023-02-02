## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

I also read:
[functional programming paradigm](https://www.geeksforgeeks.org/functional-programming-paradigm/)
as the examples in the first link were missing.

and
[Functional Programming concepts everyone should know](https://hackernoon.com/9-functional-programming-concepts-everyone-should-know-uy503u21)

#### How does this subject matter as it relates to what I am studying?

One of my goals, beyond getting the basic concepts, is to write clean, easy to understand, readable code.

### What is functional programming?

"Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia"
"A way for us to think of problems as a matter of interconnecting functions.

### What is a pure function and how do we know if something is a pure function?

* "It returns the same result if given the same arguments ( also referred to as **deterministic**)
* It does not cause any observable side effects"

### What are the benefits of a pure function?

"Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen."

### What is immutability?

It means, something cannot be changed.

*"Unchanging over time or unable to be changed."
*"When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value."

#### *Why is this important?*

"Mutation can be problematic because it makes tracing the state changes in our application hard or even impossible. You don't want to call a function in a third party library and not know if it will modify the object you're passing."-Hackernoon

### What is Referential transparency?

"Basically, if a function consistently yields the same result for the same input, it is referentially transparent."

### Advantages and Disadvantages of functional programming according to Geeks for Geeks link

**Advantages**:  

* "Pure functions are easier to understand because they don’t change any states and depend only on the input given to them. Whatever output they produce is the return value they give. Their function signature gives all the information about them i.e. their return type and their arguments.
* The ability of functional programming languages to treat functions as values and pass them to functions as parameters make the code more readable and easily understandable.
* Testing and debugging is easier. Since pure functions take only arguments and produce output, they don’t produce any changes don’t take input or produce some hidden output. They use immutable values, so it becomes easier to check some problems in programs written uses pure functions.
* It is used to implement concurrency/parallelism because pure functions don’t change variables or any other data outside of it.
* It adopts lazy evaluation which avoids repeated evaluation because the value is evaluated and stored only when it is needed.

**Disadvantages**:  

* Sometimes writing pure functions can reduce the readability of code.
* Writing programs in recursive style instead of using loops can be bit intimidating.
* Writing pure functions are easy but combining them with the rest of the application and I/O operations is a difficult task.
* Immutable values and recursion can lead to decrease in performance.

**Applications**:

* It is used in mathematical computations.
* It is needed where concurrency or parallelism is required."

Videos

## [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

### What is a module?
just Another JavaScript File

We use modules to keep our code categorized and easier to modify read both for use and other developers down the line. 

### What does the word ‘require’ do?
"Facilitates a way to include JavaScript modules in your code."
It "brings" files into another file. 

### How do we bring another module into the file the we are working in?

Use a string to create a path to the module that you require in the file .
Using the require function. 
Ie:
You have a file named fruit.js with a function named makePie() and you want to bring it into app.js. In app.js you would write:
var makeSomePie(or names can match) =require('./fruit');

in fruit.js you would need to export that function, by writing:
module.exports = makePie;

### What do we have to do to make a module

make another file. 
to connect the files, use require() in the file you are wanting to use the module. 

Use export in the module you are wanting to send. 

#### Things I want to know more about:

New Term: **Memoize**
Wiki: "In computing, memoization or memoisation is an optimization technique used primarily to speed up computer programs by storing the results of expensive function calls and returning the cached result when the same inputs occur again."
(in other words, helps speed up computations)
It sounds like memorization, but it is specific to computing. The term was coined in 1968 and derived from "memorandum" (to be remembered)
