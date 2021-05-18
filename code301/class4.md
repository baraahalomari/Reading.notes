# React Docs - Forms


## What is a ‘Controlled Component’?

A Controlled Component is one that takes its current value through props and notifies changes through callbacks 
like onChange .
A parent component "controls" it by handling the callback and managing its own state and passing 
the new values as props to the controlled component.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.


We should update them because we don't want to have a fixed value for input.

## How do we target what the user is entering if we have an event handler on an input field?

By resetting the value.

# The Conditional (Ternary) Operator Explained

 
## Why would we use a ternary operator?

Use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.


## Rewrite the following statement using a ternary statement: 
if(x===y){
   console.log(true);
  } else { 
     console.log(false); }
     

x === y? console.log(true) : console.log(fals);

