# Reading class 04

## Classes and Objects

- **Objects** are an encapsulation of variables and functions into a single entity
- Objects get their variables and functions from **classes** 
- Classes are a template for objects
- To access variable inside of a class you would follow template: var_name.class_var_name
- Access object functions: var_name.function_name
- The **__init__()** function is a special function that is called when the class is being initiated

## Thinking recursively

- A **recursive** function is a function defined in terms of itself via self-referential expressions
  - The function will continue to call itself and repeat its behavior until some condition is met to return a result
- Two parts of a recursive function:
  - Base case
  - Recursive case
- Each recursive call has its own execution context so to maintain state:
  - Thread the state through each recursive call so that the current state is part of the current call's execution 
  - Keep the state in global scope
- A list is an example of a recursive data structure
- A data structure is recursive if it can be defined in terms of a smaller version of itself
- Python doesn't have support for tail-call elimination -- a stack overflow can happen if you end up using more stack frames than the default call stack

## Things I want to know more about
- How do objects and classes in python differ from other objects and classes in javascript
- Is using recursive code similar to using loops
- What other data structures can be recursive