##  API Integration

### [Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)

#### Explain the different between a query string parameter and a path parameter.

A query string parameter is a part of the URL that is used to provide additional information to the server. It is appended to the URL after a question mark "?" and consists of key-value pairs separated by ampersands "&". Query string parameters are optional and can be used for filtering or specifying additional details.

A path parameter, on the other hand, is a dynamic part of the URL that is used to identify a specific resource or entity. It is a placeholder within the URL and is denoted by a colon ":" followed by the parameter name. Path parameters are typically used to retrieve or manipulate a specific resource.

#### What would our API URL with a path id parameter be given the following information:

Domain: http://our-site.com
v3
model name: stuff
id: things

http://our-site.com/api/v3/stuff/things

#### We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

Imagine you have an online store where you sell different products. Now, to manage your store, you need a way for your website to communicate with a special server called an API (Application Programming Interface). This API acts like a bridge between your website and your store's database, allowing them to exchange information.

Now, the cool thing about this API is that it's designed to be "model agnostic," which means it can work with any type of data model. A data model is like a blueprint that defines how your data should be structured and organized.

The API has a set of rules that it follows to understand what your website needs. It supports various operations like retrieving data (GET), creating new records (POST), updating records (PUT/PATCH), and deleting records (DELETE). It uses a standardized format called JSON (JavaScript Object Notation) to exchange data.

To use the API, your website sends requests to specific URLs (web addresses) that the API recognizes. For example, if you want to get a list of products, you would send a GET request to a URL like "our-site.com/api/v1/products". The API understands this URL structure and knows you want product data.

You can also provide additional information in the URL called parameters. There are two types: query string parameters and path parameters. Query string parameters are like filters that allow you to narrow down the data you want. For example, you can request products only in the "electronics" category by adding "?category=electronics" to the URL.

Path parameters, on the other hand, help you specify a particular entity or record. For example, if you want to retrieve a specific product with the ID "12345," you would add "/12345" to the URL.

The API then processes your requests, fetches the relevant data from the database, and sends it back to your website in a standardized format. Your website can then use this data to display products, update information, or perform any other actions it needs to provide a great shopping experience.

So, in simpler terms, the API acts as a mediator between your website and the store's database, understanding and fulfilling the requests your website makes for data. It's like a helpful assistant that ensures your website has all the information it needs to function properly.

### [Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)

#### Describe how you would use middleware to implement basic and bearer auth.

To implement basic and bearer authentication using middleware, you can configure the server to intercept incoming requests and validate the authentication credentials. For basic authentication, the middleware checks if the provided username and password match the stored credentials. For bearer authentication, the middleware verifies the validity of the provided token. If the authentication fails, the server can respond with an appropriate error message or deny access to protected resources. Middleware acts as a security layer that ensures only authenticated users can access the protected endpoints of the API.

#### Describe the handshake necessary to implement OAuth.

OAuth is an authorization protocol that allows users to grant third-party applications access to their resources on a server without sharing their credentials. The handshake process involves three parties: the user, the third-party application (client), and the server (service provider). Firstly, the client requests authorization from the user, who then authenticates with the server. After successful authentication, the server generates an access token and provides it to the client. The client can then use this access token to make authorized requests to the server on behalf of the user, without exposing the user's credentials.

#### Describe how Role Based Access Control works to a non-technical friend.

Role-Based Access Control is a system that manages access to resources based on predefined roles assigned to users. Imagine RBAC as a security system for a building. Each person is given an access card that grants different levels of access based on their role. For example, a security guard may have access to all areas, while an employee has access to their department only. In RBAC, roles are defined based on job responsibilities, and users are assigned to specific roles. This ensures that individuals have appropriate access permissions, maintaining security and preventing unauthorized access to sensitive information or functionalities.