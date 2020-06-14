## Reading 10 - June 11<sup>th</sup>

## **Duckett JS**

### Ch 10 - Error Handling & Debugging (p 449-486)
*"JavaScript can be hard to learn and everyone makes mistakes when writing it."*

- Understanding *execution contexts* and *stacks* helps to find errors in your code
  - Think through the order of execution
  - *Global context*
  - *Function context*
  - *Eval context*
- Statement needs data from another function, it *stacks* new function on top of current task
  - Good pic depicting this on pg 454
- JavaScript pretty much runs twice
- *Global scope* vs *function-level scope*
  - Ideally you'd create variables inside the functions that use them
- 7 types of built-in error objects in JavaScript
- *Debugging* involves *process of deduction*
  - Debugging workflow on pg463
  - Can use *debugger;* and then you can step around it (cool!)
- Use the console to narrow down the area where error is
- *Try* statement
  - Put code you think might bung up into a *try* block
  - If an exception occurs in this section, control is passed to *catch* block
- *Catch* statement
  - Pass error object parameter into it
  - Has alternate set of code
- *Finally* statement
  - Will run either way, whether try block succeeded or failed
- Pg 484 for **debugging tips** and **common errors**



[Back to Home](README.md)