## July 17<sup>th</sup>

### Call Stack 

https://developer.mozilla.org/en-US/docs/Glossary/Call_stack
- **Call stack** is way for interpreter to keep track of its place in script calling multiple functions 
  - Script calls function, interpreter adds to call stack and starts function
  - Functions called by that function are added to call stack further up, run when called
  - Current function finished, interpreter takes it off stack
  - If stack takes up more space, results in *stack overflow* error

https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/
- JavaScript engine is a **single-threaded** interpreter with **heap** and **single call stack**
- **Single-threaded** - can only do one thing at a time
- Function execution top to bottom, *call stack is synchronous*
- Call stack is **data structure that uses LIFO to temp store and manage function invocations**
- Stack frame is memory location in stack, cleared when function returns and leaves stack
- *Stack overflow* when there's recursive function without exit point
- **Recursive** function is one that calls itself

### Debugging

https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
- Red of error messages is the call stack
- Reference errors
  - **Temporal Dead Zone** (TMD) refers to let and const and the fact that there is time between hoisting and declaring and the reference error that occurs when you try to access them in this time
- Syntax errors
- Range errors
- Type errors
- Console.logs are our friends
- *debugger* statement
  - can also set conditional breakpoints
- Use *try* and *catch*

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors
- Helpful list of all errors and a link to further explanation