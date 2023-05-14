### Express REST API

Express is the middleware used in building MERN applications.


#### [ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

* Classes are a template for creating _**objects**___.

* Can a class declaration be hoisted?
no

* How would you describe a constructor and contextual “this” to a non-technical friend?

"A JavaScript constructor is a special function that is used to create objects. Think of it like a blueprint or a template for building objects. Just like how you might have a blueprint for a house that you use to build many houses with similar features, you can use a constructor to create many objects with similar properties and behaviors.

The "this" keyword in JavaScript is a way to refer to the current object that the code is working with. It's kind of like using "me" or "I" to refer to yourself when you're talking to someone else. In a constructor, "this" is used to refer to the object being created by the constructor. So if you have a constructor for creating a person object, for example, "this" would refer to the specific person being created each time the constructor is called." - ChatGPT


#### [Using Express Routing](https://expressjs.com/en/guide/routing.html)

* Within Express, what does routing refer to?
Routing refers to how an application’s endpoints (URIs) respond to client requests.

* What is the difference between a route path and a route method?
A **route method** is derived from one of the HTTP methods, and is attached to an instance of the express class.
**Route paths**, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

* When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?


"In a Node.js web application using a framework like Express, you can use middleware functions to handle incoming requests and prepare them for processing by the route handlers. Middleware functions can modify the request and response objects or perform other tasks, such as authentication or logging.

The next function is a parameter that is passed to a middleware function, and it is used to pass control to the next middleware function in the chain or to the final route handler. Middleware functions can use the next function to pass control to the next middleware function in the chain or to the final route handler.

It's appropriate to add next as a parameter to a route handler if you want to pass control to the next middleware function or the final route handler in the chain. For example, if you have multiple middleware functions that need to be executed before the final route handler, you can use next to pass control to the next middleware function in the chain.

If next has been passed to your middleware as a parameter, you must call it in order to pass control to the next middleware function or the final route handler. If you do not call next, the request will be left hanging and the client will eventually time out.

It's also important to make sure that you call next with an error object if an error occurs in your middleware function. This will allow error-handling middleware functions to handle the error and respond appropriately to the client. If you do not pass the error to next, the error may go unhandled and cause issues for your application." - ChatGPT


#### [Express Routing](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4)

* What is an Express Router?
"An Express Router is a middleware function that provides a way to group related routes and their associated handlers into separate modules. Routers allow you to modularize your application and keep your code organized and maintainable." -ChatGPT

* By what mean do we initialize express.Router() in an express server?

"To initialize an Express Router in an Express server, you need to first require the Express module and then call the Router() method on the Express module, like this:
const express = require('express');
const router = express.Router();" -ChatGPT

* What do we use route middleware for?

"Route middleware is like a helper that can assist the main function of your application (the route handler) by performing additional tasks before or after the route handler does its job.

For example, imagine you are a baker and you have an online bakery where customers can place orders for cakes. When a customer places an order, you need to check if they are logged in, if they have selected a cake, and if the cake is available. You could write all of these checks directly into your main function (the route handler), but this would make your code very long and difficult to manage.

Instead, you can use route middleware to perform these checks before the main function runs. This makes your code more organized and easier to maintain. The middleware functions can also be reused in other parts of your application if you need to perform the same checks elsewhere.

Another use case for route middleware is logging. You can add a middleware function that logs incoming requests and outgoing responses. This helps you to keep track of what is happening in your application and identify any issues that might arise.

Finally, route middleware can also be used for error handling. If an error occurs during processing of a request, the middleware can catch the error and return an appropriate response to the client. This helps to ensure that your application is robust and handles errors gracefully.

So, to sum up, route middleware is like a helper that can perform additional tasks before or after the main function of your application (the route handler) runs. It can be used for tasks such as authentication, input validation, logging, and error handling." -ChatGPT


#### Reflection
What are your learning goals after reading and reviewing the [class README?](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-03/)

* I want to learn how to add express routers () to break down the route handling logic.
* Use Sequelize models and schemas to perform CRUD operations.
* Testing code that relies on a Postgres Database server.

#### Things I want to know more about

* How to use a router in express. 
