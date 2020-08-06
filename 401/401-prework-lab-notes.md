## Callbacks
https://www.youtube.com/watch?v=xLDI7hIgU4o&feature=youtu.be

- "hey function, i want you to do some work, when youre done, run this function for me". when you call the callback, you give it the function to run
- callback functions are passed as an argument to another function
- mostly happens "offline" which means asynchronously 
- fs library is the File System Module for node.js
  - code knows how to read from the file system
- always plan for callback to be the single source where your code is going to run

## Promises

- "hey function, plz do your work and when you finish, .then() give ME the data and I'll handle it"
- runs like a callback but syntax is a bit more inline
- Promise constructor takes resolve and reject
- promise chaining (.then to .then to .then)
- being a good async developer is being a good javascript developer
- dont worry so much about the order in which things actually happen, worry about the order in which you deal with things
- if you care about the order, chain them
  - in one then, return something to the next .then in the chain and those things will happen in sequence with themselves (not in sequence with the things around them)
- a .then is a function that returns a promise, that ultimately with resolve or reject your request 