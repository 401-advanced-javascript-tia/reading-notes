## July 16<sup>th</sup>

### Functional Programming

https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa
- **Functional programming** is a style that treats computation as the evaluation of mathematical functions, avoids changing-state and mutable data
  - **Pure functions**
    - make it only do one thing!
    - returns same result if given same arguments (*deterministic*)
    - function that relies on random num generator is not pure
    - doesnt cause observable side effects
  - **Immutability**- *unchanging over time or unable to be change*
  - **Recursion**- *function calls itself repeatedly until it arrives at result*
    - keeps variable(s) immutable
  - **Referential transparency**
    - *pure functions* + *immutable data*
  - Functions as first-class entities
    - refer to it from constants and variables
    - pass it as parameter to other functions
    - return is as result from other functions
- This stuff blows my mind, **bookmarked, come back to this article**

### Refactoring JavaScript for Readability
https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec
- Strategies for refactoring:
  - Return early from a function
  - Cache variables so functions can be read
  - Use APIs when you can!
- Always think about refactoring, do it early
