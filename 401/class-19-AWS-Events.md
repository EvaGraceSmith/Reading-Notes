## AWS: Events


### [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

#### What is the difference betweeen SQS and SNS?

"SQS (Simple Queue Service) is a fully managed message queuing service that decouples and asynchronously processes messages between distributed systems. SNS (Simple Notification Service) is a fully managed publish/subscribe messaging service that enables message distribution to multiple recipients or endpoints.

#### What are some use cases for both SNS and SQS?


Some use cases for SNS (Simple Notification Service) include sending notifications, mobile push notifications, and triggering workflows. Use cases for SQS (Simple Queue Service) include decoupling components, processing tasks asynchronously, and handling high-volume data processing in a distributed system.

## [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

#### Describe how to use SQS and SNS in a “fanout” pattern.

In a "fanout" pattern, messages are sent to a single SNS topic, and multiple SQS queues are subscribed to that topic. Each queue receives a copy of the message, allowing for parallel processing and distribution of messages to multiple consumers or workers.

#### Explain how “push notifications” work, using SNS.


Using SNS (Simple Notification Service), push notifications work by sending messages to subscribed endpoints, such as mobile devices or applications. When a push notification is triggered, SNS delivers the message to the specified endpoints, enabling instant and real-time notifications on the receiving devices or applications.


### [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

#### How might a large scale, distributed application make use of a Queue system like SQS?


A large-scale, distributed application can use a Queue system like SQS (Simple Queue Service) to decouple components and handle asynchronous processing. It allows different parts of the application to communicate efficiently, ensuring scalability, fault tolerance, and efficient resource utilization across distributed systems." - ChatGPT


Bookmark and Review
[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)

### Reflection

#### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-19/)?

I would like to become more proficient in utilizing messages in queue.