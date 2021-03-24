# HTML Text, CSS Introduction, and Basic JavaScript Instructions

### Chapter 2 (Text)
As we learned befor that the HTML is the structre of any webpage and we use a lot of tags to writ it . now we are going to learn the types of these tags :

1. Structural markup :
    its the element that we use to describe headings and paragraphs . for example :
    - `<h1>`
    - `<p>`
    - `<b>`
    - `<i>`

2. Semantic markup :
    this provides exstra information for example :
    - `<strong>`
    - `<em>`
    - `<q>`
    - `<del>`

### Chapter 10  (Introducing CSS)
   we know that there is three ways that to write a css code :
   1. inline (inside the tag --- `<p style="color : red ;">`)
   2. enternal (we write the css code inside the head on the html file )
   3. external (we write the css code on external file )

 - but why we prefare to use the external way ?
  + we can apply it to multiple documents 
  + once we changed any thing it will reflecte on the pages that reference the stylesheet
  + more professional way 

  ### Chapter 2 (Basic JavaScript Instructions)
   
   the java script is a programming languge the we use with htmal and css to make our website alive and interactive with users 

   -  How to declare a variables on java script ?
    first write the variable keyword (**var**) then the variable name for example :
    + var name ; 
    if you want to give it value :
    + var name = "my name"; (string value)
    + var num= 5 ; (number value)
    + var question = false; (boolean value)


### Chapter 4 (Decisions and Loops)
  + if we want to write a conditioal statment we use if else , or switch statment for example :

 ```
  - if(age > 50 ){
      you are old ;
  } else if(age < 15 ){
      you are young ;
  }

```
   + if we want to run some code more than one time pased on a codition we use loops and these is three types of loops :
   1. for ---- `for(var i=0;i<10;i++){}`
   2. while ---- `while(i<10){    i++ ;}`
   3. do while ---- `do{  i++;} while (i<10)`