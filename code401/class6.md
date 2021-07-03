## Review, Research, and Discussion


### Explain what a “Singleton” is (in Computer Science terms)

is a software design pattern that restricts the instantiation of a class to one "single" instance. 

### Explain how the Singleton pattern can be used with Node modules, specifically with classes

We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

use the singleton approch.

## Document the following Vocabulary Terms



**Router Middleware** : it does actualy is to take the original request, and forward it to a sub handler according to the path.

**Dynamic Module Loading** : Function-like form of import that returns a promise of the requested module.

**Singleton Pattern** : A creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.

**CRUD -> REST Method Matches** : hese correspond to create, read, update, and delete (or CRUD) operations, respectively. 

**Mock Testing** : An approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.

## Preview

### Which 3 things had you heard about previously and now have better clarity on? 

* Singleton pattern.
* Router middleware.
* CRUD apps.

###  (Links to an external site.)Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

* Dynamic Modules. 
* Mocking the server.
*  mock testing in general.
  
### What are you most excited about trying to implement or see how it works?
Dynamic Modules.

# Securing Passwords

> Passwords are the first line of defense against cyber criminals.

We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

> Hash is the most important technique to secure passwords and is regarded to be quite safe for data or password integrity.

> Bcrypt is a function of adaptive hash based on a cryptographic Blowfish cipher symmetric block cipher method, introducing a labor factor, which can decide how costly the hah function will be, also known as security factor.


# Basic Auth

Basic access authentication is a method for an HTTP user agent to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :. 

HTTP does not provide a method for a web server to instruct the client to "log out" the user. However, there are a number of methods to clear cached credentials in certain web browsers. One of them is redirecting the user to a URL on the same domain, using credentials that are intentionally incorrect. However, this behavior is inconsistent between various browsers and browser versions. Microsoft Internet Explorer offers a dedicated JavaScript method to clear cached credentials.

# OWASP auth cheatsheet 

* Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

* Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. The Session Management Cheat Sheet contains further guidance on the best practices in this area.

* The cheatsheet also has all useful info someone might need when dealing with OWASP Auth.

# Bcrypt Docs

bcrypt is a password-hashing function designed by Niels Provos and David Mazières, based on the Blowfish cipher and presented at USENIX in 1999. Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.

> The bcrypt function is the default password hash algorithm for OpenBSD and was the default for some Linux distributions such as SUSE Linux.

> There are implementations of bcrypt for C, C++, C#, Elixir, Go, Java, JavaScript, Perl, PHP, Python, Ruby, and other languages.