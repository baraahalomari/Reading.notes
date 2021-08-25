# React Native

## Review, Research, and Discussion]

### Compare and Contrast Redux Toolkit with Redux “Ducks”

* Ducks are an alternative to having separate folders for actions/reducers/constants. It keeps redux functionality in a single file. 
* It combines reducers, actions, and constants in one file called a slice. 
* Each slice will provide an initial state and a reducer function for an object in store. It is prone to circular dependency

### What is the principle advantage of Redux Toolkit

Helps to solve three major problems with Redux: configuring a Redux store, adding numerous packages to get Redux to things, and removing unnecessary or boilerplate code.

## Document the following Vocabulary Terms

* **redux toolkit slices**  A function that accepts an initial state, an object full of reducer functions, and a “slice name”, and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.


* **namespace** A namespace is a declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries.

# Preparation Materials

> React Native is like React, but it uses native components instead of web components as building blocks.

> Most components can be customized when they are created, with different parameters. These creation parameters are called props.

**This lets you make a single component that is used in many different places in your app, with slightly different properties in each place.**


> Unlike props that are read-only and should not be modified, the state allows React components to change their output over time in response to user actions, network responses and anything else.

#### React primitives render to native platform UI, meaning your app uses the same native platform APIs other apps do.


# Expo

> **Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.**


