
## AWS Core Services

### AWS Interacting Methods
* AWS console - Web/App Based
* AWS CLI - Command line Interface
* AWS SDK - Software Developer Kit
### IAM
AWS **Identity and Access Management** (IAM) enables you to **manage access** to AWS services and resources securely. Using IAM, you can create and manage **AWS users and groups, and use permissions to allow and deny their access to AWS resources**. IAM is a feature of your AWS account offered at no additional charge. You will be charged only for use of other AWS services by your users.
## Amazon Elastic Compute Cloud (Amazon EC2) 
Is a web service that provides resizablee compute capacity in the Cloud. It is designed to make web-scale computing easier for developer. Amazon EC2 **provides different instance (as servers)** types to enable you to choose the CPU, memory, storage, and networking capacity that you need **to run your applications**.
### EC2 Use Cases
* Web application hosting
* Batch processing
* Web services end point
* Desktop in the cloud
### EC2 Core concept
* **Instace Type**: Define the processor, memory, and storage type. Catagores are:
  * General Purpose
  * Compute memory and storage optimized
  * Accelared computing 
* **Root Device Type**: Two types
  * Instance Store: if you shut down server then data will go away.
  * EBS(Elastic Block store): Data will be persistant mean if you shut down server then data is still there.
* **AMI - Amazon Machine Image**: Template for an EC2 instance including configuration, operating system and data.
* **Purchase Option**- pricing is based on instance type. Purhase options are:
  * On Demand: You pay by the second for the instance that are launched
  * Reserved: You purchase at a discount instance in advanced for 1-3 years
  * Spot: you can leverage unused EC2 capacity in a region for a large discount
## AWS Elastic Beanstalk
**Automates the process of deploying and scaling workloads on EC2 (PaaS)**
* Support a specific technologies
* Leverage existing AWS services
* Only pay for the other services you leverage
* Handle provisioning, load balancing, scaling and monitoring
#### Elastic BeanStalk Features
* Monitoring
* Deployment
* Scaling
* EC2 customization
### Elastic Beanstalk Use Cases
* Deploy an application with minimal knowledge of other services
* Reduec the overall maintenance needed for the application
* Few customizations are required

## AWS Lambda
AWS Lambda is a **serverless compute service** that lets you **run code without provisioning or managing servers**, creating workload-aware cluster scaling logic, maintaining event integrations, or managing runtimes. With Lambda, you can run code for virtually any type of application or backend service - all with zero administration. Just **upload your code as a ZIP file or container image, and Lambda automatically and precisely allocates compute execution power and runs your code based on the incoming request** or event, for any scale of traffic.

> **NOTE:** Serverless computing is a cloud computing execution model in which the **cloud provider runs the server**, and **dynamically manages the allocation of machine resources**

### Use Cases

* **Data processing**: Lambda can be directly triggered by AWS services such as S3, DynamoDB etc.
* **Real-time file processing**: You can use Amazon S3 to trigger AWS Lambda to process data immediately after an upload. 
* **Real-time stream processing**: You can use AWS Lambda and Amazon Kinesis to process real-time streaming data for application activity tracking, transaction order processing, click stream analysis, log filtering, social media analysis etc.
* **achine learning**: You can use AWS Lambda to preprocess data before feeding it to your machine learning model. 
* **Backends**: You can build serverless backends using AWS Lambda to handle web, mobile, Internet of Things (IoT), and 3rd party API requests. 
* **Web applications**: By combining AWS Lambda with other AWS services, developers can build powerful web applications that automatically scale up and down and run in a highly available configuration across multiple data centers – with zero administrative effort required for scalability, back-ups or multi-data center redundancy.

### Advantages
* Reduced maintenance requirments
* Enables fault tolerance without  additional work
* Scales based on demand
* Pricing is based on usage

#### SSM 
AWS Systems Manager or Simple System Manager is an **AWS service** that you can **use to view and control your infrastructure on AWS**. Systems Manager simplifies resource and application management, shortens the time to detect and resolve operational problems, and helps you operate and manage your AWS infrastructure securely at scale


### References:
* https://aws.amazon.com/iam/
* https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc
* https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html
* https://aws.amazon.com/lambda/
