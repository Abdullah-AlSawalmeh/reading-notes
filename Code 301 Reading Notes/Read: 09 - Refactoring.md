## Concepts of Functional Programming in Javascript

1. What is functional programming?

   - Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

2. Pure functions

   - It returns the same result if given the same arguments (it is also referred as deterministic)
   - It does not cause any observable side effects

3. Immutability

   - Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

4. Referential transparency

   - pure functions + immutable data = referential transparency

5. Functions as first-class entities

   - refer to it from constants and variables
   - pass it as a parameter to other functions
   - return it as result from other functions

6. Higher-order functions

   - takes one or more functions as arguments, or
   - returns a function as its result

7. Filter

   - The filter function expects a true or false value to determine if the element should or should not be included in the result collection.

8. Map

   - The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.

9. Reduce
   - filter by book type
   - transform the shopping cart into a collection of amount using map
   - combine all items by adding them up with reduce
