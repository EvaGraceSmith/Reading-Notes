Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.


## Readings: AWS: Cloud Servers
Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
### [AWS EC2](https://aws.amazon.com/ec2/)
___

* What is an EC2 Instance? 
"An EC2 (Elastic Compute Cloud) instance is a virtual server provided by Amazon Web Services (AWS). It is one of the core services offered by AWS and allows users to rent virtual machines in the cloud to run their applications. EC2 instances provide scalable computing capacity and can be easily provisioned and configured to meet specific requirements.

Here are some key points about EC2 instances:

1. Virtual Servers: EC2 instances are essentially virtual servers running in the cloud. They are created and managed through the AWS Management Console, AWS CLI (Command Line Interface), or SDKs (Software Development Kits).

2. Scalability: EC2 instances offer scalability, allowing users to scale up or down the number of instances based on their computing needs. This flexibility helps handle variations in workload and ensures optimal resource utilization.

3. Instance Types: AWS provides a wide range of EC2 instance types optimized for different workloads. These instance types differ in terms of computing power, memory capacity, storage capabilities, and network performance. Users can choose the most appropriate instance type for their specific application requirements.

4. Operating Systems: EC2 instances support various operating systems, including popular options like Linux and Windows. Users can select the desired operating system and configure it according to their needs.

5. Storage Options: AWS offers multiple storage options for EC2 instances, such as Amazon Elastic Block Store (EBS) for persistent block-level storage, Amazon S3 for object storage, and instance store volumes for temporary storage directly attached to the instance.

6. Networking: EC2 instances can be connected to virtual networks within AWS using Amazon Virtual Private Cloud (VPC). Users can configure network settings, security groups, and access control rules to control inbound and outbound traffic.

7. Pricing: EC2 instances follow a pay-as-you-go model, where users are billed based on the instance type, the duration of usage, and any additional resources attached to the instance (such as storage or data transfer).

EC2 instances are widely used for various purposes, including web hosting, application deployment, data processing, machine learning, and more. They provide a flexible and scalable infrastructure for running a wide range of workloads in the cloud.

* Name 2 use cases for EC2.

Web Application Hosting: EC2 instances are often used to host web applications. Users can deploy their web servers, such as Apache or Nginx, on EC2 instances and configure them to serve their web application content. EC2 instances provide the necessary computing power and scalability to handle incoming web traffic, making it easier to handle varying workloads and ensure the availability of the application.

Big Data Processing: EC2 instances are well-suited for big data processing tasks. Organizations can leverage the computational capabilities of EC2 instances to process large volumes of data using frameworks like Apache Hadoop, Apache Spark, or other data processing tools. EC2 instances can be configured in clusters to distribute the workload and speed up data processing tasks, making it easier to analyze and derive insights from large datasets.

These are just a couple of examples, but EC2 instances can be used for various other purposes such as running containerized applications, hosting databases, running machine learning models, and more. The versatility and scalability of EC2 instances make them a popular choice for a wide range of workloads in the cloud.

* Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

One reason to use Amazon Elastic Container Service (ECS) instead of services like Heroku, Digital Ocean, or Render.com is the deep integration with the broader AWS ecosystem. 

AWS offers a comprehensive suite of cloud services, including storage (Amazon S3), databases (Amazon RDS), messaging (Amazon SNS), monitoring (Amazon CloudWatch), and many others. By using ECS, which is part of AWS, you can seamlessly integrate your containerized applications with these services.

Here are a few benefits of leveraging the AWS ecosystem with ECS:

1. Full Integration: ECS allows you to easily connect your containerized applications with other AWS services. For example, you can leverage Amazon RDS for managed database services, Amazon S3 for object storage, or Amazon DynamoDB for NoSQL databases. This integration enables you to build complex and scalable architectures by leveraging the various AWS services alongside your ECS containers.

2. Scalability and Flexibility: AWS offers extensive scalability options and auto-scaling features that allow you to dynamically adjust the resources allocated to your ECS containers based on demand. You can easily scale up or down the number of containers and adjust resource allocation with AWS Auto Scaling. This level of scalability and flexibility can be beneficial for applications with varying workloads.

3. Security and Compliance: AWS has strong security measures in place, including network security, data encryption, identity and access management, and compliance certifications. By using ECS within the AWS ecosystem, you can benefit from these security measures and leverage AWS services like AWS Identity and Access Management (IAM) for access control and AWS Key Management Service (KMS) for encryption of data at rest and in transit.

4. Monitoring and Management: With ECS on AWS, you can utilize Amazon CloudWatch to monitor the performance, logs, and metrics of your containerized applications. CloudWatch provides valuable insights into the health and performance of your infrastructure, allowing you to troubleshoot and optimize your applications effectively.

While services like Heroku, Digital Ocean, and Render.com may have their own strengths and unique features, the deep integration with the extensive AWS ecosystem is a significant advantage of using ECS. It provides a rich set of services, scalability options, security features, and monitoring capabilities, allowing you to build and manage your containerized applications within a robust and comprehensive cloud environment.


[EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

* Where can we find EC2 on the AWS Console?

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


* Explain the general difference between T2 Micro and XL.

The general difference between T2 Micro and XL instances lies in their performance, compute capacity, and pricing.

1. Compute Capacity: T2 Micro and T2 XL instances belong to the T2 family of EC2 instances that are designed for general-purpose workloads and are based on a burstable performance model. However, the T2 Micro instance has lower compute capacity compared to the T2 XL instance.

- T2 Micro: The T2 Micro instance is the smallest size available in the T2 family. It provides 1 vCPU (Virtual CPU) and a moderate baseline level of CPU performance. It is suitable for lightweight applications or low-traffic workloads that do not require significant processing power.

- T2 XL: On the other hand, the T2 XL instance offers a larger compute capacity. It provides higher CPU performance with more vCPUs (typically 2 or more) and more memory compared to the T2 Micro instance. It is better suited for applications that require more processing power or handle higher traffic loads.

2. Burstable Performance: Both T2 Micro and T2 XL instances follow a burstable performance model. They have CPU credits that accumulate over time when the workload is below the baseline performance level. During periods of increased demand, the instances can use the accumulated credits to burst above the baseline performance for short durations. Once the accumulated credits are exhausted, the instances revert to the baseline performance.

3. Pricing: The pricing for T2 Micro and T2 XL instances also differs. T2 Micro instances are generally less expensive compared to T2 XL instances due to their lower compute capacity. AWS pricing is based on instance size, region, and usage, so it's important to review the AWS pricing documentation or the AWS Pricing Calculator for specific pricing details.

It's important to consider your application's resource requirements, anticipated workload, and budget when choosing between T2 Micro and T2 XL instances. If your application needs more compute capacity and can benefit from higher performance, T2 XL instances may be a better fit. However, if you have a lightweight workload with lower resource demands, T2 Micro instances may be a more cost-effective choice.


* Explain a “Compute Cycle” to a non-technical friend.


Imagine you have a task that needs to be done, like solving a math problem or processing a large amount of data. To get the task done, you need a computer or a device with processing power.

Now, a compute cycle refers to a single unit of work that the computer performs to complete a task. It's like a tiny step that the computer takes to process information or perform calculations.

Let's say you have a lot of math problems to solve. Each math problem requires multiple compute cycles to calculate the answer. So, when you input the math problem into the computer, it starts working on it by performing a series of compute cycles.

During each compute cycle, the computer performs calculations, makes decisions, and carries out instructions to move closer to the solution. It does this very quickly, going through many compute cycles in a short amount of time.

The more powerful the computer, the faster it can complete these compute cycles and solve the math problems. This is why computers with higher processing power can perform tasks more quickly and efficiently.

So, a compute cycle is like a small step that a computer takes to complete a task. By performing many compute cycles in sequence, the computer can process information, solve problems, and perform various tasks for us.


Elastic Beanstalk

* What is Elastic Beanstalk?

Elastic Beanstalk is a platform as a service (PaaS) offered by Amazon Web Services (AWS). It simplifies the process of deploying, managing, and scaling applications in the cloud. With Elastic Beanstalk, developers can focus on writing code and let AWS handle the underlying infrastructure and platform management tasks.

Here are some key points about Elastic Beanstalk:

1. Application Deployment: Elastic Beanstalk allows you to deploy web applications developed in various programming languages such as Java, .NET, PHP, Node.js, Python, Ruby, and Go. It supports popular web frameworks and automatically handles the deployment of application code, including provisioning of resources like Amazon EC2 instances, load balancers, and databases.

2. Infrastructure Management: Elastic Beanstalk abstracts away the complexity of infrastructure management. It provides a managed environment where you can simply upload your application code and Elastic Beanstalk takes care of the deployment, resource provisioning, and configuration based on best practices. This allows developers to focus more on writing code and less on infrastructure setup.

3. Scalability and Load Balancing: Elastic Beanstalk offers automatic scalability and load balancing capabilities. It can automatically scale the number of instances based on application demand, ensuring that your application can handle traffic spikes without manual intervention. Elastic Beanstalk uses AWS Auto Scaling and Elastic Load Balancing to distribute traffic and manage instances efficiently.

4. Monitoring and Logging: Elastic Beanstalk integrates with AWS services like Amazon CloudWatch, which provides monitoring and logging capabilities for your applications. You can view metrics, set alarms, and collect logs to monitor the health and performance of your applications.

5. Platform Updates: Elastic Beanstalk regularly releases platform updates, including security patches and performance enhancements. These updates are applied to the underlying infrastructure without interrupting your application. This ensures that your application stays secure and up-to-date with the latest technology stack.

6. Flexibility and Customization: Elastic Beanstalk offers flexibility to customize your application environment based on your specific requirements. You can configure various parameters, environment variables, and platform settings. Additionally, you can leverage AWS services and integrate with other AWS resources to extend the functionality of your application.

Elastic Beanstalk simplifies the process of deploying and managing applications in the AWS cloud, making it an ideal choice for developers who want to focus on writing code and rely on AWS to handle the underlying infrastructure. It provides a scalable and managed environment for running web applications without the need for manual provisioning or complex setup.


* Describe the relationship between EC2 and Elastic Beanstalk.

The relationship between EC2 (Elastic Compute Cloud) and Elastic Beanstalk can be described as follows:

EC2 is a foundational service within AWS that provides virtual servers (known as instances) in the cloud. It offers a flexible and scalable infrastructure for running various workloads. Users have full control over the EC2 instances, allowing them to customize the operating system, software, and configurations according to their needs. EC2 is highly configurable and suitable for a wide range of use cases.

Elastic Beanstalk, on the other hand, is a higher-level service provided by AWS that simplifies the deployment and management of applications in the cloud. It abstracts away the underlying infrastructure details and automates the process of deploying applications on AWS, including the provisioning of EC2 instances.

Elastic Beanstalk uses EC2 instances as the underlying compute resources for running the deployed applications. When you deploy an application using Elastic Beanstalk, it automatically provisions the necessary EC2 instances, load balancers, and other resources required to run your application. Elastic Beanstalk handles the deployment process, monitoring, and scaling of the EC2 instances based on the application's needs.

Elastic Beanstalk provides a platform layer on top of EC2, managing the application lifecycle and allowing developers to focus on writing code rather than worrying about infrastructure management. It leverages the capabilities of EC2 for compute power, scalability, and flexibility.

In summary, EC2 is a foundational service that provides the virtual server infrastructure, while Elastic Beanstalk is a higher-level service that simplifies application deployment and management by leveraging EC2 instances and other AWS resources. Elastic Beanstalk makes it easier to utilize the power of EC2 without the need for manual configuration and management, enabling developers to deploy applications quickly and efficiently.

* Name some benefits of using Elastic Beanstalk.
1. Easy Deployment: Elastic Beanstalk makes it easy to upload and deploy your applications without worrying about complicated setup or configurations.

2. Scalability: Your application can automatically handle increased traffic and workload without you having to manually manage resources.

3. Reliable and Secure: Elastic Beanstalk takes care of infrastructure updates and security patches, ensuring that your application is always up-to-date and secure.

4. Integration with AWS: You can easily connect your application to other AWS services, like databases or storage, to enhance its functionality.

5. Monitoring and Troubleshooting: Elastic Beanstalk provides monitoring and logs to help you keep track of your application's performance and quickly identify and fix issues." - ChatGPT

Bookmark and Review

[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)

### Additional Questions
____
Looking ahead at this module’s course schedule, What do you look forward to learning?
What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-16/)?

I would like to know enough to not incur huge charges from AWS.
