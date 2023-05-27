## Socket.io


Learning to process for communicating data over the internet is an important concept when building applications. 


### [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)
___

####  1. What is a Web Socket?

"A Web Socket is a computer communications protocol that allows for full-duplex communication channels over a single TCP connection. It provides a standardized way for a web browser or client application to establish a long-lived connection with a web server, enabling real-time data transfer and facilitating a two-way ongoing conversation between the client and server.

#### Describe the Web Socket request/response handshake and what happens once the connection is established.

The Web Socket request/response handshake begins with the client sending a WebSocket handshake request to the server. This request includes specific headers like Upgrade, Connection, Sec-WebSocket-Key, and Sec-WebSocket-Version. The server responds with a WebSocket handshake response, indicating a successful upgrade. This response includes headers like Upgrade, Connection, Sec-WebSocket-Accept, and possibly Sec-WebSocket-Protocol.

Once the connection is established, the client and server can communicate by sending WebSocket frames back and forth. These frames contain the actual data or messages being exchanged. The frames have a small header that includes information like the opcode (operation code), payload length, and masking key (if applicable). The payload data follows the header.
 
#### Web Sockets provide a standardized way for the server to send content to a client without first receiving a __*request*__ from that client.


### [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)
___

#### What does the event handler io.on() do?

The event handler io.on() in Socket.IO is used to listen for incoming events from clients or other sources. It allows you to define a callback function that will be executed when a specific event occurs. This event handler is typically used on the server-side to handle events triggered by clients.

#### Describe some possible proof of life or proof that the code works as expected

To ensure that the code works as expected and establish proof of life, you can perform the following checks:

* Check the server logs for any error messages or exceptions. If there are no errors, it indicates that the server is running without any critical issues.
* Verify that the client-side code successfully establishes a connection with the server. This can be checked by inspecting the client-side logs or using browser developer tools to see if the WebSocket connection is established.
* Test the functionality of different events and event handlers by triggering events from clients and verifying that the corresponding event handlers are executed on the server-side.

#### What does socket.emit() do?

The function socket.emit() is used to send a custom event from the server to a specific client or to all connected clients. It allows the server to send data or information to clients in real-time. When calling socket.emit(), you specify the event name as the first parameter, followed by any data or arguments that you want to send along with the event. The client-side code can then listen for that specific event using socket.on() and handle the received data accordingly. Essentially, socket.emit() facilitates server-to-client communication in Socket.IO.


### Socket.io vs Web Sockets
___

#### What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket and Socket.IO are both technologies used for real-time communication between clients (such as web browsers) and servers. To draw an analogy, we can think of WebSocket as the underlying technology or protocol, similar to how Git is a version control protocol. On the other hand, Socket.IO is a library built on top of WebSocket, providing additional functionalities and making it easier to work with WebSocket, similar to how GitHub provides a platform and additional features for Git or how Auth0 provides an identity management system on top of OAuth.

#### When would you use Socket.IO?

You would use Socket.IO when you want to enable real-time, bidirectional communication between a client (such as a web browser) and a web server. Socket.IO simplifies the process of working with WebSocket, allowing you to handle events and exchange data in real-time. It provides features like automatic reconnection, support for broadcasting messages to multiple clients, and handling various browser inconsistencies. Socket.IO is particularly useful for applications that require real-time updates, chat functionality, collaborative features, or live data streaming.

#### When would you use WebSockets?

WebSocket would be used when you specifically need to establish a direct, persistent, and full-duplex communication channel between a client and a server. WebSocket is a protocol that operates over a TCP connection and allows for real-time, two-way communication. It is suitable for scenarios where you want instant and continuous data exchange between the client and server without the need for repeated requests. WebSocket can be used in various applications, including real-time analytics, online gaming, collaborative editing, and financial trading systems.

In summary, WebSocket is the underlying technology providing full-duplex communication, while Socket.IO is a library built on top of WebSocket that simplifies its usage and provides additional features for real-time communication between clients and servers. Socket.IO is often preferred when working with WebSocket due to its added functionalities and easier implementation." - ChatGPT


### Videos
___
#### OSI Model Explained



##### What are a couple of key takeaways from this video?

* OSI stands for Open System Interconnection
* Defines and is used to understand how one computer transferred data to another
* It allows for different OS systems to work together. Think: Mac vs Microsoft


#### TCP Handshakes Explained

##### Translate the gist of this video to a non-technical friend

* TCP stands for transmission control protocol TCP is a reliable and a connection-oriented transport protocol
* before TCP transmits data it will use a three-way handshake to establish a connection 
* step 1 the client sends a SYN segment to the server asking for synchronization
* step 2 the server replies with SYN ACK (SYN ACK means synchronization and acknowledgement)
* step 3 the client replies with ACK which is like "yes!", then the two-week connection is established between them 




### Bookmark and Review

[Socket.io Documentation](https://socket.io/docs/v4/)

[Socket.io Server API](https://socket.io/docs/v4/server-api)

[Socket.io Client API](https://socket.io/docs/v4/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)

### Reflection

#### What are your learning goals after reading and reviewing the class README?

I would like to be able to: 
* Implement a standalone Socket.io server for handling events and real time messaging.
* Use events to properly route incoming messages and payload
