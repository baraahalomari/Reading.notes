## Review, Research, and Discussion


* Why is access control important?
Because it is a valuable security technique that can be used to regulate who or what can view or use any given resource.
*Without proper access control you could leave your staff and your company wide open to problems such as data loss, theft or breach of privacy and data protection laws.*

* Describe an application that would need access control.
Reistration system for university

* What is a role used for?
Roles are created for various job functions.

* Why is role based access control more scalable than discretionary or mandatory access control?

- Because roles can be added easily if needed.
- Actions for each role can be easily modified and will be updated for all users.
- Actions on routes can be changed easily since they are merely parameters in the middleware.

## Document the following Vocabulary Terms

* **Authorization :** Granting a user to do specific actions.
* **Role Based Access Control :** An approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control or discretionary access control.
* **Capabilities :** They are the actions (permissions) specified for each role.

## Preview


* Which 3 things had you heard about previously and now have better clarity on?
- SQL  - Authurization - Authentication

* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
Event

* What are you most excited about trying to implement or see how it works?
Crud api with auth


# Event Driven Programming

> Is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

### Concepts
* An Event Handler is a callback function that will be called when an event is triggered.
* A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter

Allows us to get started incorporating Event-Driven Programming in our project right away.

### Removing Listeners

To remove event listeners in EventEmitter we can use the **removeListener** or **removeAllListeners** method. It’s important to note that in the EventEmitter that comes built-in with Node you must pass a reference to the exact function you wish to remove when using the removeListener method.

### Object Oriented Programming + Event-Driven Programming

The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.


# Node docs: events

> **Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.**

> **All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.**




