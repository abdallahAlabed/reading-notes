# React and Forms

## HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state

## form behavior of browsing to a new page when the user submits the form. If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”

## What is a ‘Controlled Component’?

###  mutable state is typically kept in the state property of components, and only updated with setState().

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.


### When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.


## How do we target what the user is entering if we have an event handler on an input field?

### By using value attributes that have a value in the state, then saving the targeted value in the state {value: event.target.value}

## The Conditional (Ternary) Operator Explained

### Use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.

## Why would we use a ternary operator?

###  let result= ((x===y)? 'true': 'false');

## Rewrite the following statement using a ternary statement:

## resources :

* https://reactjs.org/docs/forms.html
