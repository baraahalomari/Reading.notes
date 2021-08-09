# Advanced State with Reducers

## Review, Research, and Discussion

### How can we ensure that an effect hook runs only once?

React has a built-in hook called useEffect. Hooks are used in function components. The Class component comparison to useEffect are the methods componentDidMount , componentDidUpdate .


### Can useState() update more than one state variable at the same time?

we could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.


### Is useState() synchronous?
useState and setState both are asynchronous

## Document the following Vocabulary Terms

* **State Hook :** Is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
* **Component Lifecycle :** Methods hey are invoked in a predictable order. Basically all the React component's lifecyle methods can be split in four phases: initialization, mounting, updating and unmounting.

## Preview


* Which 3 things had you heard about previously and now have better clarity on?
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
* What are you most excited about trying to implement or see how it works?

# useReducer hook

> useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. 
> useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

# Ultimate Guide to useReducer

### How does useReducer work?

* useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

* useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke. This is similar to the pattern Redux uses but with a few differences.

### The reducer function

* The reduce() method in JavaScript executes a reducer function on each element of the array an and then returns a single value. The reduce() method accepts a reducer function, which itself can accept up to four arguments. 

* The reducer function itself accepts two parameters and returns one value. The first parameter is the current state, and the second is the action. The state is the data we are manipulating. The reducer function receives an action, which is executed by a dispatch function.

### useState vs. useReducer

**Although useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.**


> In building a React app, it is important to note that no single Hook can solve all our problems. It’s all about understanding where each of the Hooks are best suited, using them accordingly, and combining different Hooks that we get to manage state in our app in a predictable fashion.

> As we’ve also discussed, the useReducer Hook may not always be the best option. It is most important to use the method that best aligns with the size and architecture of your application.

