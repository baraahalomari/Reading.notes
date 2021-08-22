# Redux - Combined Reducers


## Review, Research, and Discussion

### Why choose Redux instead of the Context API for global state?

In a large scale application, Redux is a better way to control state.

### What is the purpose of a reducer?
Process of giving someone the ability to access a resource.

### What does an action contain?
Object literals that tell the reducer what is being done to the app, and any data required for the update.

### Why do we need to copy the state in a reducer?
Reducers are not allowed to modify the existing state, instead they must make immutable updates by copying the existing state and making changes to the copied values.

## Document the following Vocabulary Terms

* **immutable state** State cannot be modified, reducers must make copies of existing state to make updates.
* **time travel in redux**  Redux DevTools records dispatched actions and the state of the Redux store at every point in time, which makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or re-starting the app.
* **action creator** Instead of creating action objects inline in the places where you dispatch actions, can create functions generating them. You might write an action creator into a separate file, and import it into your component.
* **reducer** Functions that take current state and an action as arguments, and return a new state result, (state, action) => newState.
* **dispatch**  A store holds the whole state tree of the application, the only way to change the state inside it is to dispatch an action on it.  
  

# Redux Docs: Using Combined Reducers 

* The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. 
* Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state.
*  Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

> Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

# Redux Docs: Combined Reducer Syntax

> As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.

> The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

```

rootReducer = combineReducers({potato: potatoReducer, tomato: tomatoReducer})
// This would produce the following state object
{
  potato: {
    // ... potatoes, and other state managed by the potatoReducer ...
  },
  tomato: {
    // ... tomatoes, and other state managed by the tomatoReducer, maybe some nice sauce? ...
  }
}

```

> A reducer that invokes every reducer inside the reducers object, and constructs a state object with the same shape.

**This function is mildly opinionated and is skewed towards helping beginners avoid common pitfalls. This is why it attempts to enforce some rules that you don't have to follow if you write the root reducer manually.**

