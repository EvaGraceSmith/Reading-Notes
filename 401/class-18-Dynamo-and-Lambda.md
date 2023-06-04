## Readings: AWS: API, Dynamo and Lambda

[AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)

#### What is Amazon API Gateway?

Amazon API Gateway is a fully managed service provided by Amazon Web Services (AWS) that allows developers to create, publish, maintain, monitor, and secure APIs (Application Programming Interfaces). It acts as a front door for applications, enabling seamless integration with other AWS services and external systems.

#### Why is Amazon API Gateway an important part of the Serverless ecosystem?


Amazon API Gateway plays a crucial role in the Serverless ecosystem by providing a managed gateway for serverless functions. It allows developers to expose their serverless functions as APIs, handles authorization, throttling, and request/response transformations, enabling easy integration and management of serverless architectures.

#### How does API Gateway integrate with other AWS services?

Amazon API Gateway integrates seamlessly with other AWS services by providing built-in integrations. It supports direct integration with services like AWS Lambda, AWS DynamoDB, AWS S3, and more, enabling developers to easily connect and interact with various AWS resources through their APIs.

### [AWS API Gateway](https://aws.amazon.com/api-gateway/)

#### What are the some benefits of using Amazon API Gateway?


Some benefits of using Amazon API Gateway include: easy creation and management of APIs, seamless integration with AWS services, built-in security features like authentication and authorization, scalability to handle high traffic, caching capabilities for improved performance, and detailed monitoring and logging for API analytics.

#### What two API types might you choose from?

RESTful APIs: Representational State Transfer (REST) APIs are widely used and follow a standard architectural style. They use HTTP methods like GET, POST, PUT, and DELETE to perform CRUD operations on resources, making them easy to understand, scalable, and widely supported.

GraphQL APIs: GraphQL is a query language that provides a flexible and efficient approach to querying and manipulating data. With GraphQL APIs, clients can request specific data they need, reducing over-fetching and under-fetching issues. It offers more control and flexibility to clients while optimizing network requests.

#### [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)



#### What is DynamoDB?


DynamoDB is a fully managed NoSQL database service provided by AWS. It offers high performance, scalability, and automatic scaling to handle large amounts of data. It is a key-value and document database that provides low-latency access to data and seamless integration with other AWS services.

#### Under what circumstances would you recommend DynamoDB over MongoDB?


DynamoDB is recommended over MongoDB in scenarios where scalability, automatic scaling, and high performance are crucial. It excels in handling large-scale, highly dynamic workloads, while MongoDB is a better choice when flexibility in data modeling and complex querying requirements are a priority.

### [AWS DynamoDB](https://aws.amazon.com/dynamodb/)

#### Explain to a non-technical friend how DynamoDB works.

DynamoDB is like a big, fast, and flexible storage cabinet in the cloud. It organizes data into tables, and each table contains items (like rows) with unique keys. You can add, retrieve, or delete items quickly, and it automatically scales to handle lots of data and requests without slowing down.

### [Dynamoose](https://dynamoosejs.com/getting_started/Introduction)

#### What is Dynamoose?

Dynamoose is an open-source JavaScript library that provides an easy-to-use interface for working with DynamoDB in Node.js applications. It simplifies the process of interacting with DynamoDB by providing an object modeling syntax similar to Mongoose, a popular MongoDB library, making it more intuitive for developers familiar with MongoDB.

#### What are some key features of Dynamoose?

Some key features of Dynamoose include: easy object modeling for DynamoDB, support for data validation and type checking, automatic schema creation, query building and execution, middleware support, and compatibility with existing DynamoDB tables and indexes." -ChatGPT

### Reflection

#### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-18/)?

I want to explore the features of Dynamo and Lambda