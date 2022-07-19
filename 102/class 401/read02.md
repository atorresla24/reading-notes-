# Reading class 02

## In Tests We Trust - TDD with Python

- Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code
- With TDD we need to think about tests first and it is ok for the possibility of the beginning being hard
- Explicitely explain what you want the test to do with the test name
- Structure AAA
  - **Arrange**: organize data needed to execute input
  - **Act**: execute code being tested
  - **Assert**: check if the output is the one you wanted
- The cycle is made up of three steps:
  - Write a unit test and make it fail
  - Write the feature and make the test pass
  - Refactor the code 
- When writing tets we are forced to think about design and how we can simplify it into smaller pieces
- Greatest advantage about TDD is to craft the software design first 

## If name equals main

- Python files can act as either reusable modules or standalone programs
- If python interpreter is running module as the main program it sets the special_name_variable to have a value of "__main__"
- A module is a file containing Python defintions and statments
- execute file by: python (filename).py

## What on Earth is Recursion

- Recursion works with 'n' or one variable but there is multiple variables with the same name but different values
- Each variable must be kept seperate since they each have the same name or else the values will conflict 
- From the main program it runs the code until it gains all the information it needs and then works from inside back out to gain the output
- 

## Things I want to know more about

- I want to understand more about recursion
- I want to know how can I strengthen my knowledge of TTD and create tests more naturally
- I want to be able to know more on how refactoring code works whether it means just to simplify the code or to add more specifics to it