# Understanding the JavaScript Call Stack

## What is a ‘call’?

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function.

## How many ‘calls’ can happen at once?

The maximum call stack size ranges from 10 to 50 thousand calls, The browser prevents your code from freezing the whole page by limiting the call stack.


## What does LIFO mean?

At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

**function firstFunction(){**

  **console.log("Hello from firstFunction");**

**}**

  **function secondFunction()**
 **{**

  **firstFunction();**

  **console.log("The end from secondFunction");**
**}**

**secondFunction();**


## What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.


# JavaScript error messages


## What is a ‘refrence error’?

This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

## What is a ‘syntax error’?

This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

## What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

## What is a ‘tyep error’?

This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.


## What is a breakpoint?

The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

## What does the word ‘debugger’ do in your code?

Debugging tools (called debuggers) are used to identify coding errors at various development stages.

The debugger statement stops the execution of JavaScript, and calls (if available) the debugging function. Using the debugger statement has the same function as setting a breakpoint in the code. Normally, you activate debugging in your browser with the F12 key, and select “Console” in the debugger menu.