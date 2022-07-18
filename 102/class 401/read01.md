# Reading class 01

## Pain vs Suffering

Pain is something seen as a necessity for growth. In order to grow you must go through some type of hardship. Only out of an intense need will growth be possible to achieve. This pain is something that we all need to go through if we really want to achieve massive growth in these next 2 1/2 months. 

Suffering is also pain *but* pain without purpose. It is pain that leads to nothing more than just causing more pain. 

It is important to identify why you're going through all of this pain. Identify:
1. What's your perspecitve?
2. Why are you doing this?
3. Do you want what comes at the end of this journey?
4. Are you doing this for you?

Try and find the reason why you're doing this to be able to make reason out of the pain you're going through.

Continue to grow yourself and push past the pain. 

## A beginner's guide to Big O Notation

- The Big O notation is used in CompSci to describe the performance or complexity of an algorithm
- Best way to understand Big O is to produce examples in code
- O(1) describes an algorithm that will always execute in the ame time (or space) regardless of the size of the input data set

Ex: bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}

- O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set

Ex: bool ContainsValue(IEnumerable<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
}

- O(N^2) represents an algorithm whose performance is directly proportional to the square of thr size of the input data set. Deeper nested iterations are O(N^3) and O(N^4) etc. 

Ex: bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++) 
    {
        for (var inner = 0; inner < elements.Count; inner++) 
        { 
            // Don't compare with self 
            if (outer == inner) continue;             
            
            if (elements[outer] == elements[inner]) return true; 
        }
    }    
    return false;
}

-O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. Example of this is the recursive Fibonacci sequence.
Ex: int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}

- Logarithm(O(log N)) - Binary search is a technique used to search sorted data sets by comparing the middle elements(median) against the target value. A success will return if it matches. If it is higher it will go through the upper half of the data set and continue to compare the target value to the data sets. If it is lower the same thing will happen with the lower half. The data set will continue to halve with each iteration util the value has been found or until it can no longer split the data set.

## Names and values in Python

- Python work like other languages that it is capable of working with other languages but, until it doesn't
- {var_name} = {value}
- Names can be reassigned 
- Assingment doesn't copy data
- Immutable types: ints, floats, strings, tuples
- Changing an:
  - int: rebinding
  - list: mutating
  - Lists can also be rebinded: Ex: nums = nums + [7]
  - Ints are **immutable**
- Assignment variants Ex:
  - x += y
  - x = x + y
  - x = x.__iadd__(y)

## Things I want to know more about

- I want to know more on understanding the fundamentals of Python such as defining variables and understanding immutable types to be able to get a grasp on basics
- I want to be able to use logs in my own code as I have an understanding of them but don't know how to use them in code
- I also want to learn how I can help others learn the difference between pain and suffering