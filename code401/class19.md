## Review, Research, and Discussion

### Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
* An API Gateway is “middleware” that makes available backend services to mobile, web and other external clients via a set of protocols and commonly through a set of RESTful application programming interfaces (APIs). An API Gateway makes it much simpler to develop, secure, manage, and scale endpoints by moving most of the required logic from the client, into the gateway.
* Express apps are easy to build. For a simple app, you just need to add a few routes and route handlers.
* Lambda functions use an execution role to get permission to write logs to Amazon CloudWatch Logs, and to access other services and resources.
* Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.


### List the AWS Database offerings and talk about the pros and cons of each
* **Relational** : Traditional applications, ERP, CRM, e-commerce
* **Key-value** : High-traffic web apps, e-commerce systems, gaming applications
* **In-memory** : Caching, session management, gaming leaderboards, geospatial applications
* **Document** : Content management, catalogs, user profiles
* **Wide Column** : High scale industrial apps for equipment maintenance, fleet management, and route optimization.
* **Graph** : Fraud detection, social networking, recommendation engines.
* **Time Series** : IoT applications, DevOps, industrial telemetry
* **Ledger** : Systems of record, supply chain, registrations, banking transactions.


### What’s the difference between a FIFO and a standard queue?

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers.

### How can the server be assured a message was properly received?
prepares a request with a certain attributes set and sends it to server.then getting an acknowledgement from the client

## Document the following Vocabulary Terms

* **Serverless API :**  Its is an API deployed by serverless service.
* **Triggers :** Pieces of code that will automatically respond to any events in DynamoDB Streams. Triggers allow you to build applications that will then react to any data modification made in DynamoDB tables.
* **Dynamo vs Mongo :**

  * MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.
  * DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.
  * DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.
  * DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.
  * DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.

* **Dynamoose vs Mongoose :**

The most popular solutions for NoSQL databases are MongoDB and AWS DynamoDB. Both are widely used and offer highly scalable cloud-level service. Your organization's long-term cloud strategy and business-specific application requirements will be the key factor to determine which NoSQL database will work the best.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
Dynamoose 
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
aws
### What are you most excited about trying to implement or see how it works?
Dynamoose 

# SQS and SNS Basics
> AWS is one of the biggest cloud computing platform providers. This tutorial series is for beginners to AWS. In the last article, we discussed how to create an AWS EC2 instance and access it with your local machine terminal.

### Amazon Simple Queue Service (Amazon SQS)

Amazon SQS send, store and receive messages between components without other services available. The data contained in the message is known as payload and it is protected. SQS stores messages until they are processed

### Amazon Simple Notification Service (Amazon SNS)

Amazon SNS is very similar to SQS. But SNS can send notifications-mobile push, email, SMS, to end-users. Amazon SNS follows the pub/sub-model. You can create an SNS topic, which is a channel for messages to be delivered. Then configure subscribers to the topic and publish messages to them. A subscriber can be an end-user such as SQS queue, AWS Lambda function, HTTP/HTTPS webhooks etc.



# AWS SQS vs SNS

> AWS SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue.

