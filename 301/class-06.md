## Class 06 Reading Notes - Node.js


#### How does this subject matter as it relates to what I am studying?
We are already utilizing npm and node in our labs/ assignments. This helps me better understand the what, why and how to use them in creating applications.  

### [An Introduction to Node.js on sitepoint.com](https://www.sitepoint.com/an-introduction-to-node-js/)

#### What is node.js?
 * a program we can use to execute JavaScript on our computers

#### In your own words, what is Chrome’s V8 JavaScript Engine?

    * A JavaScript compiler built by Google that is open source and built into both browsers and applications.


### What does it mean that node is a JavaScript runtime?
    * When it sees JS code, it compiles it as it runs it. 

### What is npm?
    * Node packet Manages. 
    * program that is used to mangage and update node and additional libriaries. 

### What version of node are you running on your machine?
* 19.3.0

### What version of npm are you running on your machine?
* 9.2.0

### What command would you type to install a library/package called ‘jshint’?
* npm install -g jshint

What is node used for?
to create a sensible development environment in which any modern JavaScript framework (for example, React or Angular) can run.

6 Reasons for Pair Programming

### [What are the 6 reasons for pair programming?](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

#### In your experience, which of these reasons have you found most beneficial?
* Learning from Fellow Students. Being able to talk through the code, see how others process the information. Gaining knowledge from their strength. Building rappor. All great aspects of pair programming. 


#### How does pair programming work?

* "While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code."
* Developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

## Bookmark and Review
[Geocoding API Docs](https://locationiq.com/)
[Axios docs](https://www.npmjs.com/package/axios)
[MDN async and await](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Promises)


#### Things I want to know more about:
I definitely want to study more on Node, Node.js, npm and how to best utilize these to make amazing web pages. 

[Promise in JavaScript](https://www.w3schools.com/js/js_promise.asp)

#### What is a JavaScript Promise?
""I Promise a Result!"

"Producing code" is code that can take some time

"Consuming code" is code that must wait for the result

A Promise is a JavaScript object that links producing code and consuming code"

[Using promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)

"A Promise is an object representing the eventual completion or failure of an asynchronous operation.

Essentially, a promise is a returned object to which you attach callbacks, instead of passing callbacks into a function.


"Important: Always return results, otherwise callbacks won't catch the result of a previous promise (with arrow functions, () => x is short for () => { return x; }). If the previous handler started a promise but did not return it, there's no way to track its settlement anymore, and the promise is said to be "floating".

