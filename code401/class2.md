# Express

## What’s the difference between PUT and PATCH?

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource. If the PATCH document is larger than the size of the new version of the resource sent by the PUT method then the PUT method is preferred.

## rovide links to 3 services or tools that allow you to “mock” an API for development like json-server

* Postman.
* Mocky.io .
* MockServer.

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

An API definition is often used as a baseline for automated tools. API definitions can be used to generate API documentation, code samples, and SDKs automatically. A few examples of tools that generate API documentation (static and interactive) from an API definition file are SwaggerHub and Swagger Inspector. A few examples of tools that can automatically generate sample code and SDKs from API definitions include REST United and SwaggerHub. 

## Compare and contrast SOAP and ReST

SOAP and REST both allow you to create your own API. API stands for Application Programming Interface. It makes it possible to transfer data from an application to other applications. An API receives requests and sends back responses through internet protocols such as HTTP, SMTP, and others.

Many popular websites provide public APIs for their users, for example, Google Maps has a public REST API that lets you customize Google Maps with your own content. There are also many APIs that have been created by companies for internal use.

SOAP and REST are two API styles that approach the question of data transmission from a different point of view.


## Document the following Vocabulary Terms

**Web Server** : is computer software and underlying hardware that accepts requests via HTTP, the network protocol created to distribute web pages or its secure variant HTTPS.

**Express** : is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. 

**Routing** : refers to how an application’s endpoints (URIs) respond to client requests.

**WRRC** : web request/response cycle traces how a user’s request flows through the app.

# An introduction to NodeJS and Express

**Node** : is an open-source, cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. 

Benefits of Node :

>  Code is written in "plain old JavaScript".
> The node package manager (NPM) provides access to hundreds of thousands of reusable packages. 
> It has a very active third party ecosystem and developer community.
> Node.js is portable. It is available on Microsoft Windows, macOS, Linux, Solaris, FreeBSD, OpenBSD, WebOS, and NonStop OS. 

**Express** : is the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks.

Benefits of Express:

> Write handlers for requests with different HTTP verbs at different URL paths (routes).
> Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
> Add additional request processing "middleware" at any point within the request handling pipeline.

## Importing and creating modules

A module is a JavaScript library/file that you can import into other code using Node's require() function. Express itself is a module, as are the middleware and database libraries that we use in our Express applications.

## Using asynchronous APIs

JavaScript code frequently uses asynchronous rather than synchronous APIs for operations that may take some time to complete. A synchronous API is one in which each operation must complete before the next operation can start.

## Using middleware

Middleware is used extensively in Express apps, for tasks from serving static files to error handling, to compressing HTTP responses. Whereas route functions end the HTTP request-response cycle by returning some response to the HTTP client, middleware functions typically perform some operation on the request or response and then call the next function in the "stack", which might be more middleware or a route handler. The order in which middleware is called is up to the app developer.

## Handling errors

Errors are handled by one or more special middleware functions that have four arguments, instead of the usual three: 
* err
* req
* res
* next

## Using databases

Express apps can use any database mechanism supported by Node (Express itself doesn't define any specific additional behavior/requirements for database management). There are many options, including PostgreSQL, MySQL, Redis, SQLite, MongoDB, etc.

# What is NPM?

Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

npm consists of three distinct components:

* the website
* the Command Line Interface (CLI)
* the registry

We Use npm to :

* Adapt packages of code for your apps, or incorporate packages as they are.
* Download standalone tools you can use right away.
* Run packages without downloading using npx.
* Share code with any npm user, anywhere.
* Restrict code to specific developers.

# What is TDD?

**“Test-driven development”** refers to a style of programming in which three activities are tightly interwoven: coding, testing and design .

## Benefits

* many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort

* the same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases

* although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling

# CI/CD

The "CI" in CI/CD always refers to continuous integration, which is an automation process for developers. Successful CI means new code changes to an app are regularly built, tested, and merged to a shared repository. It’s a solution to the problem of having too many branches of an app in development at once that might conflict with each other.