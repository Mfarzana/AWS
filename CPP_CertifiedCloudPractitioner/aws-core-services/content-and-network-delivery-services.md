# Networking and Content Delivery Services

## Amazon Virtual Private Cloud (Amazon VPC)
is a service that lets you launch AWS resources in a logically isolated virtual network that you define
* Enables virtual networks in AWS
* Support **IPv4 and IPv6**
* Allows for **configuration of**
  * IP address range
  * **Subnets**
  * **Route Tables**
  * **Network gateway**
* Support public and private subnets
* Can utilize **NAT** for private subnets
* Enable a connection to your data center
* Can connect to other VPC's
* Support private connection to many AWS services
## AWS Direct Connect
AWS Direct Connect is a cloud service solution that makes it easy to establish a dedicated network connection from your data center ato AWS

## Amazon Route 53
**Amazon Route 53 is a** highly available and scalable cloud **Domain Name System (DNS) web service**. It is designed to give developers and businesses an extremely reliable and cost effective way to route end users to Internet applications by **translating names like www.example.com into the numeric IP addresses like 192.0.2.1** that computers use to connect to each other. 
* **Domain Name service (DNS)**
* Global AWS Service(Not Regional)
* Highly Avaialble
* Enable Global Resouce Routing
> **NOTE**: Route 53 does not require region selection
## Elastic Load Balancing
Elastic Load Balancing **automatically distributes** incoming application **traffic across multiple targets**, such as **Amazon EC2 instances, containers, IP addresses, Lambda functions, and virtual appliances**. Supports one or more AZ's in a region.
### Three types of load balancer
* Application Load Balancer (ALB)
* Network Load Balancer (NLB)
* Classic Load Balancer
## Scaling on Amazon EC2
* **Vertical Scaling or Scale up**:  You scale up your instance type to a large instance type with additional resources
* **Horizontal scaling or Scale Out**: You scale out and additional instances to handle the demand of your application.

```diff
! Scaling up** is when you change the instance types within your Auto Scaling Group to a higher type. 
For example: changing an instance from a m4.large to a m4.xlarge, scaling down is to do the reverse.

! Scaling out is when you add more instances to your Auto Scaling Group and 
scaling in is when you reduce the number of instances in your Auto Scaling Group.

For example: Let's say you have an ASG with 4x m4.xlarge instances. 
If one fails that means you lost 25% of your processing capability.
However if you had say 8x m4.large instead, your total compute is the same as 4x m4.xlarge
however if 1 instance dies then you only lose 12.5% of your resources.
! Typically its better to use more smaller instances than less larger ones.
```
## Amazon CloudFront
is a fast **content delivery network (CDN) service** that securely ***delivers data, videos, applications, and APIs to customers** globally with low latency, high transfer speeds, all within a developer-friendly environment.
* Content Delivery Network (CDN)
* Enables **users to get content from servers closet to them**
* Support static and dynamic content
* Utilizes AWS edge locations
* Include advance security features
  * AWS shield for DDoS
  * AWS WAF (Web Application Firewall)
## Amazon API Gatway
* Fully managed API management services
* Direct integrates with AWS multile services
* Provide monitoring and metrices for api all
* Support VPC and on-premise private applications
> Using API Gateway, **you can create RESTful APIs and WebSocket APIs** that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.
## References
* https://aws.amazon.com/vpc/?vpc-blogs.sort-by=item.additionalFields.createdDate&vpc-blogs.sort-order=desc
* https://aws.amazon.com/directconnect/
* https://aws.amazon.com/route53/
* https://aws.amazon.com/elasticloadbalancing/?elb-whats-new.sort-by=item.additionalFields.postDateTime&elb-whats-new.sort-order=desc
* https://stackoverflow.com/questions/42034688/aws-scale-out-scale-up#:~:text=Scaling%20out%20is%20when%20you,an%20ASG%20with%204x%20m4.
* https://aws.amazon.com/cloudfront/
* https://aws.amazon.com/api-gateway/
