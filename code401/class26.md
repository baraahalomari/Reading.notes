## Review, Research, and Discussion

### Name 5 Javascript UI Frameworks (other than React)

> Sencha Ext JS

> Angular

> Vue

> Ember

> Svelte

### What’s the difference between a framework and a library?

The key difference between JavaScript libraries and frameworks is that libraries consist of functions that an application can call to perform a task, while a framework defines how a developer designs an application. In other words, the framework calls on the application code, rather than the other way around. Of course, developers still need libraries to accomplish basic tasks on the web using JavaScript.

## Document the following Vocabulary Terms

* **Rendering :**  is the displaying of the code onto the webpage
* **Templates :** Templating refers to the client side data binding method implemented with the JavaScript language.
* **State :** State describes the status of the entire program or an individual object. It could be text, a number, a boolean, or another data type. It's a common tool for coordinating code. 

## Preview


### Which 3 things had you heard about previously and now have better clarity on?
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
### What are you most excited about trying to implement or see how it works?


# react hello world

>  ReactDOM is a package that provides DOM specific methods that can be used at the top level of a web app to enable an efficient way of managing DOM elements of the web page.

ReactDOM.render(
  &lt;h1>Hello, world!&lt;/h1>,

  document.getElementById('root')
);



# introducing JSX

>  it is a syntax extension to JavaScript. using it with React to describe what the UI should look like. JSX comes with the full power of JavaScript.

> React doesn’t require using JSX.
>  JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

> **Since JSX is closer to JavaScript than to HTML, React DOM uses camelCase property naming convention instead of HTML attribute names.**

> If a tag is empty, you may close it immediately with />.



# rendering elements

> Applications built with just React usually have a single root DOM node. 

> **To render a React element into a root DOM node, pass both to ReactDOM.render()**

>**React elements are immutable. Once you create an element, you can’t change its children or attributes.**

> **The only way to update the UI is to create a new element, and pass it to ReactDOM.render().**

> React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

> 
