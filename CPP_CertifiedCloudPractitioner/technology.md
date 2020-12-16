
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
* **Purchase Option**- pricing is based on instance type.

#### SSM 
AWS Systems Manager or Simple System Manager is an **AWS service** that you can **use to view and control your infrastructure on AWS**. Systems Manager simplifies resource and application management, shortens the time to detect and resolve operational problems, and helps you operate and manage your AWS infrastructure securely at scale


### References:
* https://aws.amazon.com/iam/
* https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc
* https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html
