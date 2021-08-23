# Redux - Asynchronous Actions

## Review, Research, and Discussion

### How granular should your reducers be?

* We can see who is sitting where during the matches, see which seats are sold when, get a list of normal buyers as well as season pass holders and many other things. Once we select a seat we can add a season pass holder manually.
* change of any of those attributes would trigger a separate kind of action such as CHANGE_EMAIL or CHANGE_NAME. And sometimes such granularity is good and valuable because different reducers, different parts of your application might need to react differently to those actions. Sometimes it might be much easier for reducers if they can distinguish between those two particular use-cases.
* But sometimes, on the other hand, this is just boilerplate. And not a single part of your app cares whether all those attributes were changed together or not. In such case, you might want to simplify your solution by dispatching just one action with all the attributes.

### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

It is a con.

### Name a strategy for preventing the above

redux thunk

## Document the following Vocabulary Terms

* **store** is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.


* **combined reducers** The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

# async actions

Asynchronous Redux Actions with Redux Thunk
* There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.
* Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.
* Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.
* The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.



# thunk middleware

> Redux Middleware and Side Effects
* By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

* A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function.

* Some common kinds of side effects are things like:

> Logging a value to the console
> Saving a file
> Setting an async timer
> Making an AJAX HTTP request
> Modifying some state that exists outside of a function, or mutating arguments to a function
> Generating random numbers or unique random IDs (such as Math.random() or Date.now())
> Redux middleware were designed to enable writing logic that has side effects.




# redux thunk

>  Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

> Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

