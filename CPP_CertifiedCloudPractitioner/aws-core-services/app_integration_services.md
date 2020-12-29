# App Integration service
**Application integration on AWS is a suite of services that enable communication between decoupled components within microservices, distributed systems, and serverless applications.**

## Amazon Simple Notification Service(SNS)
Amazon Simple Notification Service **(Amazon SNS) is a managed service that provides message delivery from publishers to subscribers** ( also known as producers and consumers ). The publisher communicates asynchronously with the recipient by sending messages to topics that are logical access points and communication channels . **Clients subscribe to SNS topics and receive issued messages using supported protocols such as Amazon SQS, AWS Lambda, HTTP, email, mobile push notifications, and mobile text messages (SMS).**

* **Fully managed pub/sub messaging service**
* Enables you to create decoupled applications
* Organized according to topic
* Integrates with multiple AWS services
* **Provides end user notifications across SMS, Email, and push notificaitons**.

![ SNS ](https://github.com/Mfarzana/AWS/blob/main/imges/sns.jpg)
### Common Amazon SNS scenarios
* Fan out
* Application and system alerts
* Push emails and text messages
* Mobile push notification
* Message durability
> Fan out-Parallel asynchronous processing

## Amazon Simple Queue Service(SQS)
Amazon Simple Queue Service **(SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications**. SQS eliminates the complexity and overhead associated with managing and **operating message oriented middleware, and empowers developers** to focus on differentiating work. **Using SQS, you can send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available**.

* **Fully managed message queue service**
* Enables you to build decoupled and fault tolerant applications
* Support up to 256 KB data payload
* **Allows message to be stored up to 14 days**
* **Provides two types of queue**
	* Standard queue
	* FIFO queue (first in first out)

## AWS Step Functions
**AWS Step Functions is a serverless function** orchestrator **that makes it easy to sequence AWS Lambda functions and multiple AWS services into business-critical applications**. Through its visual interface, you can create and run a series of checkpointed and event-driven workflows that maintain the application state. **The output of one step acts as an input to the next. Each step in your application executes in order, as defined by your business logic**.

* Enable orchestration of workflows through a fully managed service
* Support servlerless architectures
* Can Support complext workflows including error handling
* Charged per state transition along with the other AWS service leveraged
* Workflows are defined using Amazon states languages

![ AWS Step Function  ](https://github.com/Mfarzana/AWS/blob/main/imges/aws_step_fn.png)

### AWS Step Function Integrations
* Compute services
* Database services
* Messaging services
* Data Processing services
* Machine learing services

## Refereces
* https://docs.aws.amazon.com/ja_jp/sns/latest/dg/welcome.html
* https://qiita.com/fjisdahgaiuerua/items/2f79042570903416d612#%E4%B8%80%E8%88%AC%E7%9A%84%E3%81%AA-amazon-sns-%E3%82%B7%E3%83%8A%E3%83%AA%E3%82%AA
* https://aws.amazon.com/sqs/
* https://aws.amazon.com/step-functions/?step-functions.sort-by=item.additionalFields.postDateTime&step-functions.sort-order=desc
