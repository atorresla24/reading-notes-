# Reading 10

## Understanding the JavaScript Call Stack

1. A call is a single, function(s) execution
2. Only one call function can be made at a time
3. LIFO means Last In, First Out
4. function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
5. Stack Overflow is caused by a recursive function without an exit point

## JavaScript error messages

1. A reference error is when you try to use a variable that is not yet declared
2. A syntax error is when you have something that cannot be parsed in terms of syntax
3. A range error is when you try to manipulate an object with some kind of length and give it an  invalid length 
4. A type error is when the types you are trying to use or access are incompatible
5. A breakpoint is achieved by putting a debugger statement in your code in th eline you want to break
6. The word debugger will trigger a breakpoint in the line of code it is placed in

## Things I want to know more about

Knowing how to use JavaScript error messages to help me fix my code
