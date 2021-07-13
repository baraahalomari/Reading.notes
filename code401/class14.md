## Review, Research, and Discussion


### What’s the difference between a FIFO and a standard queue?

FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.

### How can the server be assured a message was properly received?

By receiving afeedback from the clint by socket.io acknowledgment.

### What classic design pattern is best represented by event driven programming?

The Observer Design Pattern defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically. Encapsulate the core (or common or engine) components in a Subject abstraction and the variable (or optional or user interface) components in an Observer hierarchy. The “View” part of Model-View-Controller.

### How do you test an event driven system?

Using jest, we can mock some event emits and test against event handlers. If we receive an acknowledgment from the client, the test will pass. Otherwise, it needs fixes.

## Document the following Vocabulary Terms

**FIFO Queue** : (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical.


**Pub/Sub**: is an asynchronous messaging service that decouples services that produce events from services.

## Preview


### Which 3 things had you heard about previously and now have better clarity on?

* Event Driven Programming. * Call Stack. * Sockets.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

The complexities of Socket Io and other uses, Building a chat between 2 people, building a fully operation all that renders and updates information realtime

### What are you most excited about trying to implement or see how it works?

Rendering and updating apps in real time

# AWS SNS and SQS

> Amazon Simple Queue Service (SQS) and Amazon SNS are both messaging services within AWS, which provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates.

