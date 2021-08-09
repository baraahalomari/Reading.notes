## Review, Research, and Discussion


### Why do we not need more .html pages in a multi-page React app?
because a single-page website can not always represent complete information.

### If we wanted a component to show up on every page, where would we put it and why?

 Inside a &lt;Route /> 

### What does routing do with the components that were rendered when a new route is requested
show new componetnt and remove the old one

### What does props.children contain?
Value that we return from the component.

### How do useState() and this.setState() differ?
setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Document the following Vocabulary Terms

* **State Hook :** The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component

* **Mounting and Un-Mounting :** 
    * Mounting: is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components).
    * Un-Mounting: This method is called just before the component gets destroyed. Any clean up statements should be executed inside this method.

### Preview


* Which 3 things had you heard about previously and now have better clarity on?
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
* What are you most excited about trying to implement or see how it works?

# effects hook

* **What does useEffect do?** By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed , and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

* **Why is useEffect called inside a component?** lacing useEffect inside the component lets us access the count state variable right from the effect. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

* **Does useEffect run after every render? :**  Yes! By default, it runs both after the first render and after every update. Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.




