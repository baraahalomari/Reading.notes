## Review, Research, and Discussion


### How does React differ from vanilla JS/HTML/CSS?

Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.

### What is the primary difference between a function component and a class component?

* A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.
* A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

## Document the following Vocabulary Terms

* **Functional Components :**  basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. 
* **Children / Child Components :** children is a special property of React components which contains any child elements defined within the component.

## Preview


### Which 3 things had you heard about previously and now have better clarity on?
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
### What are you most excited about trying to implement or see how it works?


# making sense of hooks

**What is a Hook?** A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.

> Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components. 

> Unlike patterns like render props or higher-order components, Hooks don’t introduce unnecessary nesting into your component tree. 

**If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications.**

> The Hooks proposal doesn’t include any breaking changes.

### Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.

> Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component. 

## So What About Classes?

They are also sufficient for defining components in general, as they provide us with all the necessary features like state. This is why we’d like Hooks to become the primary way to define React components in the future.


# the state hook

If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. We’re going to do that right now!

> useState is a new way to use the exact same capabilities that this.state provides in a class. Normally, variables “disappear” when the function exits but state variables are preserved by React.

> Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need.

>  useState returns a pair of values: the current state and a function that updates it.


# hooks api

> useState is a Hook 

**React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else. It’s similar to this.setState in a class, except it doesn’t merge the old and new state together.**

> The only argument to useState is the initial state

> The array destructuring syntax lets us give different names to the state variables we declared by calling useState.

**Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes .**

>  Hooks are a way to reuse stateful logic, not state itself. In fact, each call to a Hook has a completely isolated state — so you can even use the same custom Hook twice in one component.


# hooks api reference

* useState

const [state, setState] = useState(initialState);

**Functional updates :**


If the new state is computed using the previous state, you can pass a function to setState. The function will receive the previous value, and return an updated value.

**Timing of effects :**

Unlike componentDidMount and componentDidUpdate, the function passed to useEffect fires after layout and paint, during a deferred event. This makes it suitable for the many common side effects, like setting up subscriptions and event handlers, because most types of work shouldn’t block the browser from updating the screen.

* **useContext**

Accepts a context object (the value returned from React.createContext) and returns the current context value for that context. The current context value is determined by the value prop of the nearest <MyContext.Provider> above the calling component in the tree.

* **useCallback**

Pass an inline callback and an array of dependencies. useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed. This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders.

