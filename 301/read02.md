# State and Props

## What are component lifecycle events?

###  React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states. Mounting, Updating, and Unmounting are the three phases of the component lifecycle.

### Mounting

### When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

## Updating

### Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order. 
### static getDerivedStateFromProps, shouldComponentUpdate, render,getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

## Unmounting

### The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

## constructor()

### The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance. Let’s take a look at some example code.


## Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary. Doing this will ignore all updates to props, so it shouldn’t be done unless it is intentional.

## static `getDerivedStateFromProps()`
### This method exists for rare cases where the state relies on changes in props over time.

## render()

### Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. Here is an example of using render.

# Q1 :Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

## render => ‘componentDidMount’

# Q2 What is the very first thing to happen in the lifecycle of React?

## Mounting : getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount 

# Q3 : Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

## ## constructor , render ,componentDidMounts,React Update,componentWillUnmount

# What does componentDidMount do?

## 

# What types of things can you pass in the props?

## The values can be any data type, from strings to functions, objects, etc 

# What is the big difference between props and state?

## Basically, the difference is that state is something like attributes in OOP : it's something local to a class (component), used to better describe it. Props are like parameters - they are passed to a component from the caller of a component (the parent) : as if you called a function with certain parameters.

# When do we re-render our application?

## React components automatically re-render whenever there is a change in their state or props. A simple update of the state, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.

# What are some examples of things that we could store in state?

## In React , whenever we are working with any data, we always use state for storing that data which may be a string , number or any complex object

## resources :

* https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093
* w3schools
* https://www.educative.io/edpresso/how-to-force-a-react-component-to-re-render
* https://blog.devgenius.io/when-its-not-good-to-use-state-for-storing-data-in-react-adcf261e8467
