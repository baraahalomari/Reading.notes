## Review, Research, and Discussion


### What does it mean that web sockets are bidirectional? Why is this useful?

Bidirectional means that it works both ways, meaning that both parties can send and receive at the same time.

### Does socket.io use HTTP? Why?

Yes , to allow HTTP and websocket servers to co-exist on the same TCP port.

### What happens when a client emits an event?

Execuiting the ebe=vent handler.

### What happens when a server emits an event?

All listening clients will execute the handler for that event.

### What happens if a client “misses” an event?

the handler woudln’t be executed.

### How can we mitigate this?

using messaging queueing.

## Document the following Vocabulary Terms

* **Socket:** A network socket is a software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network.

* **Web Socket:** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

* **Socket.io:** is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js. Both components have a nearly identical API.

* **Client:** is a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. The server is often (but not always) on another computer system, in which case the client accesses the service by way of a network.

* **Server:** is a piece of computer hardware or software that provides functionality for other programs or devices, called “clients”.

* **OSI Model:** is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology.

* **TCP Model:** is the conceptual model and set of communications protocols used in the Internet and similar computer networks. It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol and the Internet Protocol.

* **TCP:** The Transmission Control Protocol is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol.

* **UDP:** In computer networking, the User Datagram Protocol is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol network.

* **Packets:** is a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload.

## Preview


### Which 3 things had you heard about previously and now have better clarity on?

* Clients. * Servers. * and Socket.io.
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

OSI and TCP 

### What are you most excited about trying to implement or see how it works?

Working with creating servers and clients and making them optimal!


# Socket.io Chat Example

> Writing a chat application with popular web applications stacks like LAMP (PHP) has normally been very hard. It involves polling the server for changes, keeping track of timestamps, and it’s a lot slower than it should be.

> The first goal is to set up a simple HTML webpage that serves out a form and a list of messages.

**Emitting events** : The main idea behind Socket.IO is that you can send and receive any events you want, with any data you want. Any objects that can be encoded as JSON will do, and binary data is supported too.

# Rooms and Namespaces

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients.

**Default room**


Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.

**Disconnection**

Upon disconnection, sockets leave all the channels they were part of automatically, and no special teardown is needed on your part.

