# Java Primitives versus Objects:


# **Exceptions in Java:**

### *  An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

### * Creating an exception object and handing it to the runtime system is called throwing an exception.

### * The call stack is the ordered list of methods that had been called to get to the method where the error occurred.

### *  Using exceptions to manage errors has some advantages over traditional error management techniques.

### * 3 Kinds of Exceptions:
  * **checked exception:** 
  These are exceptional
  ### conditions that a well*written application should anticipate and recover from and they are subject to the Catch or Specify Requirement.
  ### * **unchecked exceptions:**
    ### * **error:** These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from and they are not subject to the Catch or Specify Requirement
    ### * **runtime exception:** These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from and they are not subject to the Catch or Specify Requirement.

# **Using Scanner to read in a file in Java:**

### *  Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type

### * Scanner also supports tokens for all of the Java language's primitive types (except for char).


### * The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing, example:

java
  Integer j = 1;          // autoboxing
  int i = new Integer(1); // unboxing
  

### Primitive variables of these types live in the stack and hence are accessed fast and the reference types are objects, they live on the heap and are relatively slow to access 

 ### * Default values:
* null For the wrapper classes
* false for the boolean type
* 0 for numeric types
 * \u0000 for the char type
  
### *  The primitive types are much faster and require much less memory. Therefore, we might want to prefer using them.



