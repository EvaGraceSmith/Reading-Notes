
## Reading
### [Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

Also read: [Callbacks](https://codeburst.io/javascript-what-the-heck-is-a-callback-aba4da2deced)

"It’s not that JavaScript didn’t execute our functions in the order we wanted it to, it’s instead that JavaScript didn’t wait for a response from first() before moving on to execute second()."

" you can’t just call one function after another and hope they execute in the right order."

"**Callbacks** are a way to make sure certain code doesn’t execute until other code has already finished execution."


#### What is a ‘call’?

* an invocation, in this context, of a function.

#### How many ‘calls’ can happen at once?

* one


#### What does LIFO mean?

* Last In, First Out
* which  "means that the last function that gets pushed into the stack is the first to be pop out, when the function returns."

#### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
A call stack is a to do list 

the call stack is an ordered set of
stack frames. It's a to-do list for function calls or invocations. The bottom of the stack
is the first function invoked.

Imagine a stack of books. The first function is the book on the bottom of the pile, the next function invoked is second, etc.

The last function (or book) on the pile is the first one to be removed. If you tried to remove a bottom book, you would get jenga. 



#### What causes a Stack Overflow?
Exceeding the number of frames allowed in the call stack
An infinite loop. Anything that runs to the point it fills up memory. 

#### [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

#### What is a ‘reference error’?

"This is as simple as when you try to use a variable that is not yet declared you get this type of errors."

#### What is a ‘syntax error’?

"this occurs when you have something that cannot be parsed in terms of syntax"

#### What is a ‘range error’?

"Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up."

#### What is a ‘type error’?

"when the types (number, string and so on) you are trying to use or access are incompatible"

#### What is a breakpoint?
Placing a stop point in your code to see what is happening.

#### What does the word ‘debugger’ do in your code?
"when running the code  you can see the “history” before reaching that breakpoint"


## Bookmark and Review
### JavaScript errors reference on MDN

#### How does this subject matter as it relates to what I am studying?
Learning to debug your code is a huge part of programming. Getting comfortable with it and learning to do it well is important. 

"Being able to read error messages and practising debugging is one of your biggest weapons has a developer, do it frequently and with enough time you will notice a great decrease in the time you spend on each error that you find along the way." 


#### Things I want to know more about:

[More on Node.js](https://www.youtube.com/watch?v=zb3Qk8SG5Ms)
 Computers can not directly run JS or compile it down to Machine code. 

 We pass JS through v8 (a c++) to compile it. 

 Node.js is a program written in c++ that wraps around v8 (also written in c++) and is 
 It takes JS, Runs it through the v8 compiler and compiles our JS into machine code. 
 Reads and write files
 connect to a database
 Act as a server for content.
 It allows me to run JS on the front end and the backend, something I wouldn't be able to do without node..I would have to use a backend server language.