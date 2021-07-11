## Review, Research, and Discussion

###  What is the benefit of transforming data into packets?

Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is “dropped,” only the dropped packet needs to be resent.

### UDP is often refereed to as a connectionless protocol. Why is this?



> UDP stand for User Datagram Protocol, and the answer is UDP is a connectionless protocol. No connection needs to be established between the source and destination before you transmit data.

> UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itself. source (Links to an external site.). UDP is commonly used for applications that are lossy (can handle some packet loss), such as streaming audio and video. It is also used for query-response applications, such as DNS queries.

### Can a socket server application have multiple socket connections?

The server can handle 65,536 sockets per single IP address. So the quantity can be easily extended by adding additional network interfaces to a server. Meanwhile, it’s extremely important to track how many connections present on a server.

### Can a socket connection application be connected to multiple socket servers?

Yes, each listening (bound) port is serviced by a separate socket (as are all the connections made from each listening port).

### Can an application be both a socket server and a socket connection?

 yes

## Document the following Vocabulary Terms

* **Observer Pattern:** is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

* **Listener:** A procedure or a function that waits for an event or a connection to occur, and then responds accordingly.

* **Event Handler:** You can define Event handlers, scripts that are automatically executed when an event occurs. Event handlers are embedded in documents as attributes of HTML tags to which you assign JavaScript code to execute.

* **Event Driven Programming:** is when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system.

* **Event Loop:** It is a construct that allows JavaScript and Node.js to perform non-blocking operations, it handles the synchronous script on a single thread, while leaving async code to be handled separately off the single thread, then adds it back to the call stack once it returns giving the impression of a multi-threaded language. Or, async code can be awaited, giving it the impression of synchronous code.

* **Event Queue:** An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

* **Call Stack:** A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, et

* **Emit/Raise/Trigger:** firing the event

* **Subscribe:** It means enrolling in a service or agreeing to receive continuous info from a publisher, the user should input their emails or some credentials to become subscribed.

* **database:** is an organized collection of data, generally stored and accessed electronically from a computer system.

## Preview


### Which 3 things had you heard about previously and now have better clarity on?
Event
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
Socket.io
### What are you most excited about trying to implement or see how it works?
Socket.io


# OSI Model Explained

> The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.

# TCP Handshakes Explained

> TCP uses a three-way handshake to establish a reliable connection. The connection is full duplex, and both sides synchronize (SYN) and acknowledge (ACK) each other. The exchange of these four flags is performed in three steps—SYN, SYN-ACK, and ACK—
