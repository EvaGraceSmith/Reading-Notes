## Message Queues

"To this point, we’ve built servers based on internal event processing and network event handling in Real Time with Socket.io. In this class, we’ll be exploring ways to “Queue” messages for guaranteed delivery"


### [Socket.io Chat Example](https://socket.io/get-started/chat/)
___

#### Explain to a non-technical recruiter what the Chat Example (above) does.


"The Chat Example is a basic chat application that allows users to communicate in real-time. It uses Node.JS and Socket.IO technologies to enable bi-directional communication between the client (web browser) and the server.

When a user sends a chat message, the server receives it and then pushes the message to all other connected clients. This means that each user can see the messages sent by other users in real-time without having to manually refresh the page or wait for server responses.

#### What proof of life are we getting on the backend from the above app?

The backend of the app provides a "proof of life" by emitting events to the server console. When a user connects to the chat application, a message saying "a user connected" is displayed in the server console. Similarly, when a user disconnects, a message saying "user disconnected" is logged.

#### Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

To send an event to everyone except for a certain emitting socket, we can use the broadcast flag in Socket.IO. In the example, the code snippet socket.broadcast.emit('hi'); is used to send a message to all connected sockets except the socket that triggered the event. This allows excluding a specific user from receiving the message while sending it to all others.

Overall, the Chat Example demonstrates how to build a simple chat application using Node.JS, Socket.IO, and basic HTML. It showcases the power of real-time communication between clients and the server, providing an interactive and seamless chat experience.


### [Rooms](https://socket.io/docs/v4/rooms)

#### What is a room and how might a room be useful?


A room is like a virtual space or channel where different users or devices can join and communicate with each other. It's a way to group sockets (connections) together based on a specific purpose or criteria.

#### How do you join a room?

Joining a room is simple. When a user or device connects to a server using Socket.IO, they can call the "join" method and specify the name of the room they want to join. For example, if you want to join a room called "some room," you would write code like this:

`socket.join("some room")`

#### how do you leave a room?

Leaving a room is similar to joining. When a user or device wants to leave a room, they can call the "leave" method and provide the name of the room they want to leave. For example, to leave the "some room" you joined earlier, you would use code like this:

`socket.leave("some room");`

### [Namespaces](https://socket.io/docs/v4/namespaces/)

#### What is a Namespace and what does it allow you to do?


A Namespace is a way to divide the functionality of your application into separate communication channels within a shared connection. It allows you to organize and isolate different parts of your application's logic, events, and rooms.

#### Each namespace potentially has its own what? (hint: 3 things)

1. Each namespace has its own event handlers, which are functions that define how the server should respond to specific events received from clients. For example, in a namespace called "/orders," you can have event handlers for events like "order:list" and "order:create." Similarly, in a namespace called "/users," you can have event handlers for events like "user:list."

2. Namespaces also have their own rooms. Rooms are groups of sockets (connections) that can receive specific events. For example, you can have a room called "room1" in the "/orders" namespace and another room called "room1" in the "/users" namespace. Events emitted to a specific room will only be received by sockets that have joined that room within the corresponding namespace.

3. Additionally, namespaces support the use of middlewares. Middlewares are functions that can intercept and modify the behavior of incoming events or perform certain actions before or after an event is handled. Middlewares are useful for tasks such as authentication or data manipulation.

#### Discuss a possible use case for separate namespaces

One possible use case for separate namespaces is when you want to create a special namespace that only authorized users have access to. By using a separate namespace, you can separate the logic related to authorized users from the rest of the application. For example, you can create an "/admin" namespace where only administrators can connect and perform administrative tasks like deleting users. This helps keep the code organized and ensures that only authorized users can access certain functionality.

In summary, a Namespace allows you to divide the functionality of your application into separate communication channels within a shared connection. It helps you organize events, rooms, and middlewares for different parts of your application. Separate namespaces can be useful for isolating functionality for specific user groups or roles." - ChatGPT

### Bookmark and Review

[Socket.io Emit Cheatsheet](https://socket.io/docs/v4/emit-cheatsheet/)

### Reflection

#### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-13/)?

I want to be able to describe and define both ordered and unordered messaging queues. 

I want to be able to build an event based messaging server. 


