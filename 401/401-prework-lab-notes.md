## Callbacks
https://www.youtube.com/watch?v=xLDI7hIgU4o&feature=youtu.be

- "hey function, i want you to do some work, when youre done, run this function for me". when you call the callback, you give it the function to run
- callback functions are passed as an argument to another function
- mostly happens "offline" which means asynchronously 
- fs library is the File System Module for node.js
  - code knows how to read from the file system
- always plan for callback to be the single source where your code is going to run

## Promises
https://www.youtube.com/watch?v=4bPdjAerRzQ&feature=youtu.be

- "hey function, plz do your work and when you finish, .then() give ME the data and I'll handle it"
- runs like a callback but syntax is a bit more inline
- Promise constructor takes resolve and reject
- promise chaining (.then to .then to .then)
- being a good async developer is being a good javascript developer
- dont worry so much about the order in which things actually happen, worry about the order in which you deal with things
- if you care about the order, chain them
  - in one then, return something to the next .then in the chain and those things will happen in sequence with themselves (not in sequence with the things around them)
- a .then is a function that returns a promise, that ultimately with resolve or reject your request 

## Async/Await
https://www.youtube.com/watch?v=o1B395-3Elg&feature=youtu.be

- "hey javascript, this function is going to be asynchronous. when it runs, I'm going to wait until the long task finishes. and then I'll take care of it inline"
- another way to work with promises that is inline, same kind of stuff going on in the background
- an async function retuns a promise. you cannot return the value from an async function
- asynchronous things will run, they will enter the callback queue in the order in which they complete, not the order in which they were created
- use a try/catch for errors 
- await is only valid in an async function 
- the function that wraps the await needs to have 'async' out front of it
- can also use these types of functions to fetch remote data
- Promise.all to collect results if you're worried about things happening at a certain time



**Callbacks, promises, and async/await are three methods to do asyn operations in JS, each different type of syntax and different set of issues/gotchas. All handle managing the event loop. Don't have to worry about when they come back, just that they do come back.** 

**Whenever you write a promise, you should practice rewriting it as something asynchronous (async/await)**


## ES6 Classes
https://www.youtube.com/watch?v=9Yc5J3Ap9-4&feature=youtu.be

- using prototype methods on constructors takes up way less memore than creating a function within the constructor
- syntax of writing a class wtih ES6 is much smoother than doing the same in constructors 
- pretty powerful tool, especially when it comes to React and Angular



