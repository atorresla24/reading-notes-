# Class 06 reading notes:

## What is the hardest thing about writing code?

* Common answers:
  - Learning a new technology
  - Naming things
  - Testing your code
  - Debugging
  - Fixing bugs
  - Making a software maintainable

* By creating a familiar problem domain it was easier to teach the new technology and for it to be learnt
* Writing code is a lot like putting together a jigsaw puzzle
* Code is put together with the purpose of building components that have been taken out of the "bigger picture"
* Issue is that many problem domains are like a puzzle with a blurry picture or no picture at all
* If the problem domain is too difficult to understand, you can make it easier by:
  - Making the problem domain easier 
  - Get better at understanding problem domains
* To make the problem domain easier you could focus on a more specific part of the problem and try and tackle that


## What's the difference between primitive values and object references in JavaScript?

* All data types in JavaScript can be classified as either:
  - primitive values
  - object references
* They differentiate in behavior

### JavaScript's 8 data types:

* Boolean
* Null
* Unidentified
* Number
* BigInt
* String
* Symbol

* When a primitive value is assigned to a variable the variable is set to that value directl
* When a variable is assigned to a object, the variable contains a reference to it

## Difference between immutable and mutable data

* Primitive values are immutable (values cannot be changed)
* Object references are mutable (values can be changed)

## Chapter 3: Object Literals

### What is an object:

* A variable that is assigned to an object is called a property
* Functions become known as methods 
* Properties or methods are accessed through dot notation 

## Chapter 5: Document Object Model

* Document Object Model specifies how browsers should create a model of an HTML page
* DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes
* You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax
* Whenever a DOM query can return more than one node, it will always return a NodeList
* From an element node you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques
* An element node can contain multiple text nodes and child elements that are siblings of each other
* In older browsers, implementaion of the DOM is inconsistent 
* Browsers offer tools for viewing the DOM tree