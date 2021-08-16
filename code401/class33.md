# &lt;Login /> and &lt;Auth />


## Review, Research, and Discussion

### Why is the Context API useful?

It can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props.


### Can a component outside of a provider get its context?

It can get global context, cannot get Context.Provider.


### What are some common use cases for using the Context API?

Currently authenticated user, or theme settings for the application.

### Describe “Context Hell”

Context API has virtually no boilerplate in comparison to Redux, adding Context Providers makes for messy and unreadable code.

## Document the following Vocabulary Terms

* **global state** Keeping a state at the top level of an application and providing access methods to all child levels without the need to pass props. Global state should only keep states that concern the entire app, such as theme, language, or other app-wide settings.
* **global context** Context provides a way to share values and data between components without having to explicity pass a prop through every level of the tree. Designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
* **provider** Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.
* **consumer** Consumers are decendants of a Provider that will re-render whenever the Provider’s value prop changes. The propagation from Provider to its descendant consumers (including .contextType and useContext) is not subject to the shouldComponentUpdate method, so the consumer is updated even when an ancestor component skips an update.

### Preview

* Which 3 things had you heard about previously and now have better clarity on?
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
* What are you most excited about trying to implement or see how it works?


# what is role based access control?

> Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

>  You can designate whether the user is an administrator, a specialist user, or an end-user, and align roles and access permissions with your employees’ positions in the organization. Permissions are allocated only with enough access as needed for employees to do their jobs.

### Some of the designations in an RBAC tool can include

* Management role scope – it limits what objects the role group is allowed to manage.
* Management role group – you can add and remove members.
* Management role – these are the types of tasks that can be performed by a specific role group.
* Management role assignment – this links a role to a role group.


## BENEFITS OF RBAC

* Reducing administrative work and IT support. 
* Maximizing operational efficiency. 
* Improving compliance.


### BEST PRACTICES FOR IMPLEMENTING RBAC

* **Current Status**: Create a list of every software, hardware and app that has some sort of security. For most of these things, it will be a password.

* **Current Roles**: Even if you do not have a formal roster and list of roles, determining what each individual team member does may only take a little discussion.

* **Write a Policy:** Any changes made need to be written for all current and future employees to see. 


[react-cookies component](https://www.npmjs.com/package/react-cookies)


[react-cookie library](https://www.npmjs.com/package/react-cookie)