


## AWS: Cloud Servers

### [AWS EC2](https://aws.amazon.com/ec2/)
___

#### What is an EC2 Instance? 

An EC2 (Elastic Compute Cloud) Instance is a virtual server provided by AWS that allows users to run applications and services on the cloud. It offers various configurations of CPU, memory, storage, and networking, allowing users to select the appropriate instance type to meet their specific computing needs.

#### Name 2 use cases for EC2.

1. Web Application Hosting

2. Big Data Processing

These are just a couple of examples, but EC2 instances can be used for various other purposes such as running containerized applications, hosting databases, running machine learning models, and more. The versatility and scalability of EC2 instances make them a popular choice for a wide range of workloads in the cloud.

#### Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

One reason to use ECS (Elastic Container Service) instead of other services like Heroku, Digital Ocean, or Render.com is the flexibility and control it provides over infrastructure. ECS allows fine-grained customization and integration with other AWS services, making it suitable for complex and highly customizable containerized applications.


[EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

#### Where can we find EC2 on the AWS Console?

To find EC2 on the AWS Management Console, you can follow these steps:

1. Sign in to the AWS Management Console at https://console.aws.amazon.com/.
2. Once you're logged in, you'll land on the AWS Management Console homepage.
3. In the search bar at the top, type "EC2" or "Elastic Compute Cloud" and press Enter.
4. The search results will display various services related to EC2. Look for "EC2 - Virtual Servers in the Cloud" and click on it.
5. You will be redirected to the EC2 Dashboard, where you can manage your EC2 instances, security groups, key pairs, volumes, and other related resources.

Alternatively, you can also locate EC2 by navigating through the AWS services. Here's another way to find EC2:

1. From the AWS Management Console homepage, locate the "Services" dropdown menu in the top navigation bar.
2. Hover over the menu, and a list of various AWS services will appear.
3. Scroll down or use the search bar within the dropdown menu to find "Compute" or "EC2."
4. Click on "EC2 - Virtual Servers in the Cloud" from the dropdown menu or search results.
5. You will be directed to the EC2 Dashboard, where you can manage your EC2 resources.

The specific appearance and layout of the AWS Management Console may vary slightly based on updates or customization, but these steps should guide you to find EC2 and access the EC2 Dashboard for managing your virtual servers in the cloud.


#### Explain the general difference between T2 Micro and XL.

The general difference between T2 Micro and XL instances lies in their performance, compute capacity, and pricing.

T2 Micro is a low-cost, entry-level instance designed for applications with low to moderate CPU usage. It provides a single vCPU and limited burstable performance using CPU credits. T2 Micro instances are suitable for small-scale applications, testing, and development environments.

On the other hand, XL refers to a larger instance size with higher specifications. XL instances offer more CPU power, memory, and storage capacity compared to T2 Micro. They are typically used for resource-intensive workloads, large-scale applications, databases, and production environments that require higher performance and scalability. XL instances are suitable for handling more significant workloads and demanding applications.

If your application needs more compute capacity and can benefit from higher performance, T2 XL instances may be a better fit. However, if you have a lightweight workload with lower resource demands, T2 Micro instances may be a more cost-effective choice.


#### Explain a “Compute Cycle” to a non-technical friend.


Imagine you have a task that needs to be done, like solving a math problem or processing a large amount of data. To get the task done, you need a computer or a device with processing power.

Now, a compute cycle refers to a single unit of work that the computer performs to complete a task. It's like a tiny step that the computer takes to process information or perform calculations.

Let's say you have a lot of math problems to solve. Each math problem requires multiple compute cycles to calculate the answer. So, when you input the math problem into the computer, it starts working on it by performing a series of compute cycles.

During each compute cycle, the computer performs calculations, makes decisions, and carries out instructions to move closer to the solution. It does this very quickly, going through many compute cycles in a short amount of time.

The more powerful the computer, the faster it can complete these compute cycles and solve the math problems. This is why computers with higher processing power can perform tasks more quickly and efficiently.

So, a compute cycle is like a small step that a computer takes to complete a task. By performing many compute cycles in sequence, the computer can process information, solve problems, and perform various tasks for us.


### Elastic Beanstalk

#### What is Elastic Beanstalk?

Elastic Beanstalk is a platform as a service (PaaS) offered by Amazon Web Services (AWS). It simplifies the process of deploying, managing, and scaling applications in the cloud. With Elastic Beanstalk, developers can focus on writing code and let AWS handle the underlying infrastructure and platform management tasks.

##### Here are some key points about Elastic Beanstalk:

1. Application Deployment: Elastic Beanstalk allows you to deploy web applications developed in various programming languages such as Java, .NET, PHP, Node.js, Python, Ruby, and Go. It supports popular web frameworks and automatically handles the deployment of application code, including provisioning of resources like Amazon EC2 instances, load balancers, and databases.

2. Infrastructure Management: Elastic Beanstalk abstracts away the complexity of infrastructure management. It provides a managed environment where you can simply upload your application code and Elastic Beanstalk takes care of the deployment, resource provisioning, and configuration based on best practices. This allows developers to focus more on writing code and less on infrastructure setup.

3. Scalability and Load Balancing: Elastic Beanstalk offers automatic scalability and load balancing capabilities. It can automatically scale the number of instances based on application demand, ensuring that your application can handle traffic spikes without manual intervention. Elastic Beanstalk uses AWS Auto Scaling and Elastic Load Balancing to distribute traffic and manage instances efficiently.

4. Monitoring and Logging: Elastic Beanstalk integrates with AWS services like Amazon CloudWatch, which provides monitoring and logging capabilities for your applications. You can view metrics, set alarms, and collect logs to monitor the health and performance of your applications.

5. Platform Updates: Elastic Beanstalk regularly releases platform updates, including security patches and performance enhancements. These updates are applied to the underlying infrastructure without interrupting your application. This ensures that your application stays secure and up-to-date with the latest technology stack.

6. Flexibility and Customization: Elastic Beanstalk offers flexibility to customize your application environment based on your specific requirements. You can configure various parameters, environment variables, and platform settings. Additionally, you can leverage AWS services and integrate with other AWS resources to extend the functionality of your application.

Elastic Beanstalk simplifies the process of deploying and managing applications in the AWS cloud, making it an ideal choice for developers who want to focus on writing code and rely on AWS to handle the underlying infrastructure. It provides a scalable and managed environment for running web applications without the need for manual provisioning or complex setup.


#### Describe the relationship between EC2 and Elastic Beanstalk.


EC2 (Elastic Compute Cloud) is a web service that provides resizable compute capacity in the cloud. Elastic Beanstalk is a platform-as-a-service (PaaS) offering by AWS that automates the deployment and management of applications on EC2 instances, simplifying the process of deploying and scaling applications.

#### Name some benefits of using Elastic Beanstalk.

1. Easy Deployment: Elastic Beanstalk makes it easy to upload and deploy your applications without worrying about complicated setup or configurations.

2. Scalability: Your application can automatically handle increased traffic and workload without you having to manually manage resources.

3. Reliable and Secure: Elastic Beanstalk takes care of infrastructure updates and security patches, ensuring that your application is always up-to-date and secure.

4. Integration with AWS: You can easily connect your application to other AWS services, like databases or storage, to enhance its functionality.

5. Monitoring and Troubleshooting: Elastic Beanstalk provides monitoring and logs to help you keep track of your application's performance and quickly identify and fix issues." - ChatGPT

### Bookmark and Review

[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)

### Additional Questions
____

What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-16/)?

I would like to know enough to not incur huge charges from AWS.
