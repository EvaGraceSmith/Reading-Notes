### JavaScript Object Basics

**How would you describe an object to a non-technical friend you grew up with?**
"In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. A cup is an object, with properties. A cup has a color, a design, weight, a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics."
[](-https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#:~:text=In%20JavaScript%2C%20an%20object%20is,properties%2C%20which%20define%20their%20characteristics.)

**What are some advantages to creating object literals?**
"The advantages of using object literals to create objects include convenience, flexibility in declaration, and less code during declaration. You can drop an object literal anywhere in your program with no previous setup and it'll work, which can be very handy!"
[](https://codeburst.io/object-oriented-programming-in-javascript-51b2bdfdfe9f#:~:text=The%20advantages%20of%20using%20object,which%20can%20be%20very%20handy!)

**How do objects differ from arrays?**
"Objects represent “things” with characteristics (aka properties), while arrays create and store lists of data in a single variable."
[](https://medium.com/@zac_heisey/objects-vs-arrays-42601ff79421#:~:text=Objects%20represent%20%E2%80%9Cthings%E2%80%9D%20with%20characteristics,data%20in%20a%20single%20variable.)

**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**

"When working with bracket notation, property identifiers only have to be a String. They can include any characters, including spaces. Variables may also be used as long as the variable resolves to a String.

This means there are fewer limitations when working with bracket notation. We can now have spaces in our strings, and can even start strings with numbers.

***Perhaps most importantly, we can now use variables to access properties in an object.*** It’s important the variable you are using references a String."

[bracket.vs.dot.notation](https://codeburst.io/javascript-quickie-dot-notation-vs-bracket-notation-333641c0f781?gi=45aebe51a8ef)



**Evaluate the code below. What does the term this refer to and what is the advantage to using this?**

const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

The this keyword refers to the current object the code is being written inside — so in this case this is equivalent to dog

"This isn't hugely useful when you are writing out object literals by hand, but it will be essential when we start using constructors to create more than one object from a single object definition, and that's the subject of the next section."

### Introduction To The DOM

**What is the DOM?**
"The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web."

"The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page."

**Briefly describe the relationship between the DOM and JavaScript.**

"As an object-oriented representation of the web page, it can be modified with a scripting language such as JavaScript."

[DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

Great Job interview article. Making sure you have mastered the code language, and how to start solving a problem:
[problem solving](https://simpleprogrammer.com/solving-problems-breaking-it-down/)

"Any language you expect to be able to solve algorithm type problems in, you should know how to do the following things:

* Create a list
* Sort a list or array
* Create a map or dictionary
* Loop through a list, or dictionary
* Parse strings
* Convert from string to int, int to string, etc"

**What’s the Difference Between Primitive Values and Object References in JavaScript?**

[](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

"JavaScript currently supports eight different data types. This includes seven primitive value types and objects. Here’s the full list.

* Boolean
* Null
* Undefined
* Number
* BigInt
* String
* Symbol
* Objects
If you are new to JavaScript this list may look strange to you: arrays, functions, and dates are all missing.

This isn’t a mistake. Arrays, functions, and dates all play an important role in JavaScript programs, but they are really just objects under the hood."

Answer: "primitive values cannot be changed (or mutated), but object references can be changed."