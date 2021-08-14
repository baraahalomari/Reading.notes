# Context API

## Review, Research, and Discussion

### Describe use cases useState() vs useReducer()
Although useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.

### Why do custom hooks need the use prefix?
Custom hooks are normal JS functions, named with the prefix ‘use’, that can use hooks inside of it and contain a common stateful logic to be reused in other components.

### What do custom hooks usually do?
Have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

### Using any list of custom hooks, research and name one that you think will be useful in your applications
useScript React hook , This hook makes it super easy to dynamically load an external script and know when its loaded.

### Describe how a hook that fetches API data might work
The effect hook called useEffect is used to fetch the data with axios from the API and to set the data in the local state of the component with the state hook's update function. The promise resolving happens with async/await. However, when you run your application, you should stumble into a nasty loop.

## Document the following Vocabulary Terms

* **reducer :** 
A function that determines changes to an application’s state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application’s state changes in a single store so that they behave consistently.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
### What are you most excited about trying to implement or see how it works?


# context api

> Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

### When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. 

> Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

> This inversion of control can make your code cleaner in many cases by reducing the amount of props you need to pass through your application and giving more control to the root components.

> This pattern is sufficient for many cases when you need to decouple a child from its immediate parents. You can take it even further with render props if the child needs to communicate with the parent before rendering.

### Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.




# hooks and context example

**From an engineering standpoint, our snackbar system must easy to use and generally be very lightweight. We want to be able to place one on the screen with just a couple of lines of code.**

#### Globally Accessible

```
export const SnackBarContext = createContext()

export function SnackBarProvider({ children }) {
  const [alerts, setAlerts] = useState([])

  return (
    <SnackBarContext.Provider value={{ setAlerts }}>
      {children}
      {alerts.map((alert) => <SnackBar key={alert}>{alert}</SnackBar>)}
    </SnackBarContext.Provider>
  )
}
```

