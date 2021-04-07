# Error Handling & Debugging

Everyone makes mistakes when writing a code in JavaScript.The errorVmessages that a browser gives look cryptic at first, but they can help you determine whatVwent wrong in your JavaScript and how to fix it.


The JavaScript interpreter uses the concept of execution contexts.VThere is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.


## EXECUTION CONTEXT

**Types of execution contexts:**

* Global context: There is only one global context in any page.
* Function Context:Each function has its own function context.
* Eval context: Text is executed like code in an internal function.

**The stack**

When a statement needs data from another function, it stacks or piles the new function on top of the current task.

## Executing context & Hoisting 

Each time a script enters a new execution context, there are two phases of activity:
> Prepare

> Execute


**Hoisting:** The abbility to Call functions before they have been declared and Assign a value to a variable that has not yet been declared.

Each execution context also creates its own variab1es object. Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.for each execution context, the scope is the
current execution context's variables object, plus the variables object for each parent execution context.

If a variable is not found in the variables object for the current execution context, it can look in the
variables object of the parent execution context.

Each time a function is called, it gets its own execution context and var i ables object.


## Understanding Errors

you can use a set of statements to handle the error, If you are anticipating that something in your code
may cause an error. if the error is not handled the script will just stop processing and the user will not know why. 

**Error Objects** 

Error objects can help you find where your mistakes are and browsers have tools to help you read them.

**Property:**

> name : Type of execution

> message : Description

> fileNumber : Name of the JavaScript file

> lineNumber : Line number of error Object

> Error : Generic error - the other errors are all based upon this error

> Syntax Error : Syntax has not been followed

> Ref erenceError : Tried to reference a variable that is not declared/within scope

> TypeError : An unexpected data type that cannot be coerced

> RangeError : Numbers not in acceptable range

> URIError : encodeURI ().decodeURI(),and similar methods used incorrectly

> EvalError : eval () function used incorrectly



## A Debugging Workflow

**Debugging is about deduction:** eliminating potential causes of an error.
first, Look at the error message, then Check how far the script is running.finally Use breakpoints where things are going wrong.

They let you pause execution and inspect the values that are stored in variables.

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.


Writing from the script to the consol Browsers that have a console have a console object, which has several
methods that your script can use to display data in the console.

To differentiate between the types of messages you write to the console, you can use three different methods. They
use various colors and icons to distinguish them.

* conso1e.info() : used for general information
* console.warn() : used for warnings
* console.error() : used to hold errors 

If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.