## Packages and Import

### packages:
 all java classes grouped togather inside it (directory)

- should start with packge decleration: 
    - package statment 
    - imports 
    - class , one public class in the same file 

### import Option
1. import package.*;  // Make all classes visible altho only one is used.
2. import package.className;  // Make a single class visible.
3. Alternately we can the fully qualified class name without an import.

#### NOTES :
- All classes in the java.lang package are visible without an import.
- import only tells the compiler where to look for symbols.
- The wildcard "*" only makes the classes in this package visible, not any of the subpackages.
- The search for names is very efficient so there is no effective difference.

## Different types of loops in Java

> looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

* types of loops:

- Do-While loop:
 first condition evaluation happens after the first iteration of the loop.

- While loop:
repeats a statement or a block of statements while its controlling Boolean-expression is true.:

- Simple for loop : 
control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.