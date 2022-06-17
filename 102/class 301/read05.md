# Reading 05

## React Docs - Thinking in React

1. The single responsibility principle is a technique that say a component should ideally only do one thing and if it ends up growing it should be decomposed to do one into smaller subcomponents. 
2. By building a 'static' version of the application means to not use state at all.
3. Once you have a static application you need to add state
4. Three questions you can ask yourself to determine if something is state are: 
- Is is passed in from a parent via props?
- Does it remain unchanged over time?
- Can you compute it based on any other state or props in your component?
5. You can identify where a state needs to live by:
- Identify ever component that renders something based on that state
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Higher-Order Functions

1. A higher-order function is a function that operates on other functions either by taking them as arguments or by returning them.
2. Line 2 of the greaterThan function is returning m is greater than n.
3. Map or reduce operates in regards to higher-order functions by interacting and altering the original array and returning a completely different array

## Things I want to know more about

So is it possible to create an application simply by using props only?