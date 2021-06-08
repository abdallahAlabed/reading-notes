# Passing Functions as Props

## Lists 

### List is the most versatile data type available in functional programming languages used to store a collection of similar data items. The concept is similar to arrays in object-oriented programming. List items can be written in a square bracket separated by commas.

## Keys

### Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

## What does .map() return?

#### map() function. We return a <li> element for each item

## If I want to loop through an array and display each value in JSX, how do I do that in React?

### You can build collections of elements and include them in JSX using curly braces {}./ using the JavaScript map() function.

## Each list item needs a unique ____.

### Key

## What is the purpose of a key?

### Keys help React identify which items have changed, are added, or are removed.

## What is the spread operator?

### JavaScript, spread syntax refers to the use of an ellipsis of three dots  to expand an iterable object into the list of arguments.

## List 4 things that the spread operator can do.

### *adding items to arrays
### * combining arrays 
### * combining objects
### * and spreading an array out into a function’s arguments

## Give an example of using the spread operator to combine two arrays.

### const num1 = ['1','2','3']
### const num2 = ['4', '5', ...num1]
### console.log(num2) //  Array(5) [ "4", "5", "1", "2", "3" ]

## Give an example of using the spread operator to add a new item to an array.

### const num1 = ['1','2','3','4','5']
### const num2 = [...num1];
### console.log(num2) // Array(5) [ "6", "7", "8", "9", "10" ]
### num1[0] = 'abdallah'
### console.log(...[...num1,'...',...num2]) //  abdallah 2 3 4 5 ... 6 7 8 9 10

## Give an example of using the spread operator to combine two objects into one.

### const objectOne = {a: "a"}
### const objectTwo = {b: "b"}
### const objectThree = {...objectOne, ...objectTwo, c: "c"}
### console.log(objectThree) // Object { a: "a", b: "b", c: "c" }
### const objectFour = {...objectOne, ...objectTwo, c: () => {console.log("c".repeat(5))}}
### objectFour.c() // ccccc 

## How to Pass Functions Between Components

### props

## In the video, what is the first step that the developer does to pass functions between components?

### super(props)

## In your own words, what does the increment function do?

### it adds value to the existing value

## How can you pass a method from a parent component into a child component?

### super(props)

## How does the child component invoke a method that was passed to it from a parent component?

### super(props)

## resources :

* https://reactjs.org/docs/lists-and-keys.html

* https://www.tutorialspoint.com/functional_programming/functional_programming_lists.htm#:~:text=List%20is%20the%20most%20versatile,square%20bracket%20separated%20by%20commas.

* https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab