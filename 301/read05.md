# Putting it all together


## How would you break a mock into a component hierarchy?
 ###  draw boxes around every component and, And take the advice of a designer who works in a special way, decomposed into smaller subcomponents also, Separate your UI into components

## What is the single responsibility principle and how does it apply to components?  
 
 ### it's a component that should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

## What does it mean to build a ‘static’ version of your application?  

 ### it's a library of reusable components that render your data model. The components will only have `render()` methods that mean The UI has no interactivity and requires a lot of typing and no thinking, and we can pass data in Static using props. props are a way of passing data from parent to child

## Once you have a static application, what do you need to add? 
 ###  add a new component in the hierarchy above the common owner component.

## What are the three questions you can ask to determine if something is the state?

 ### Is it passed in from a parent via props? If so, it probably isn’t state.
 ### Does it remain unchanged over time? If so, it probably isn’t state.
 ### Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where the state needs to live?
 ###  The first state lives in FilterableProductTable because The common owner component is FilterableProductTable and if we need to identify where the state lives we may note that do decide:
 ### ProductTable needs to filter the product list based on state and SearchBar needs to display the search text and checked state.
 ### It conceptually makes sense for the filter text and checked value to live in `FilterableProductTable`

 ## resources :
 https://reactjs.org/docs/thinking-in-react.html