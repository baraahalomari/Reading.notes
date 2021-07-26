## Review, Research, and Discussion

* **What are serverless functions?**
  
A serverless function is a programmatic function written by a software developer for a single purpose. It’s then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

* **If you were to create a system that emulated Lambda functions, how would you do it?**
* Open the Functions page on the Lambda console.

* Choose Create function.

* Describe how a CDN works

## Document the following Vocabulary Terms

* **Serverless Functions :**serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. The engineering teams within those companies ensure that the serverless functions have near-perfect uptime, redundant instances around the world, and scale to any incoming network request volume.
  
* **Cloud Storage :**is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access.

* **CDN :**refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content.

## Preview

* Which 3 things had you heard about previously and now have better clarity on?
aws

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
aws

* What are you most excited about trying to implement or see how it works?
aws


# AWS API Gateway Overview
> Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.


> API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

## Benefits of Amazon API Gateway
* Map HTTP requests to specific functions in a Serverless application viaanAPI Gateway event. 
* Map WebSocket events to Serverless functions. 
* Use multiple microservices to serve the same top-level API. 
* Save time with integrations: authentication, developer portal, CloudTrail, CloudWatch.

> The AWS free tier includes one million (1M) REST API calls per month for the first 12 months of each new AWS account. The WebSocket API free tier is 1M messages and 750,000 connection minutes per month, also for the first 12 months.


# AWS API Gateway

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications.

# AWS DynamoDB Guide

> DynamoDB is a hosted NoSQL database offered by Amazon Web Services 

## Use cases

* Applications with large amounts of data and strict latency requirements.
* Serverless applications using AWS Lambda.
* Data sets with simple, known access patterns.


# AWS DynamoDB

> Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. 

## Benefits

* Performance at scale
* No servers to manage
* Enterprise ready

## Applications

* Applications
* Mobile Backends
* Microservices


# Dynamoose

> Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

## Key Features

* Type safety
* High level API
* Easy to use syntax
* Ability to transform data before saving or retrieving documents
* Strict data modeling (validation, required attributes, and more)
* Support for DynamoDB Transactions
* Powerful Conditional/Filtering Support
* Callback & Promise support