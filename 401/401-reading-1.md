## Aug 9<sup>th</sup>

### 1. Why would you want to run JavaScript code outside of a browser?

- To run JavaScript code outside of a browser you would need to utilize Node.js. Being able to run JS outside of the browser means we can interact with databases and create APIs! It allows us to do what other languages (like C and Python) were already doing is being able to use that language for outside-the-browser stuff. 

### 2. What is the difference between a module and a package?

- A module is just a single JavaScript file whereas a package contains one or more modules along with a package.json file that contains information (*metadata*) about that package.  

### 3. What does the node package manager do?

- Node package manager is what we use to be able to utilize the tools/packages of Node.js. It installs them and provides the interface to be able to work with them.   

### 4. Provide code snippets showing 3 different ways to export a function from a node module

```
module.exports = {};
```

```
module.exports = functionName;
```

```
module.exports.functionName = functionName;
```


| **Term**      | **Definition** |
| ------------- | -------------- |
| **ecosystem**     | collection of things that are developed and evolve in the same environment       |
| **Node.js**       | JS runtime. JS running on the server. fast because it uses non-blocking I/O        |
| **V8 Engine**     | Chrome's runtime JS engine that parses and executes script code. Written in C++        |
| **module**        | self-contained, single JavaScript unit with functionality. can be used on the server side        |
| **package**       | bits of reusable code, shared via npm. directory with one or more modules in it and a package.json with metadata about the package     |
| **node package manager (npm)**   | world's largest software registry, used to share and borrow packages. way to reuse code from other developers, and a way to share your code with them        |
| **server**        | system that accepts and responds to requests made over a network (receives requests for web file and sends that to the client)       |
| **environment**   | state of a computer- software, hardware, and running programs       |
| **interpreter**   | one part of the js engine. translates line by line into something the machine can understand        |
| **compiler**      | other part of the js engine. the program that translates (compiles) code into something the machine can understand and execute (*bytecode*). it does this ahead of time, as opposed to an interpreter that goes line by line        |


**Resources:**
- https://docs.npmjs.com/about-npm/index.html
- https://www.youtube.com/watch?v=U8XF6AFGqlc&feature=emb_rel_end
- https://developers.google.com/apps-script/guides/v8-runtime
- https://stackoverflow.com/questions/20008442/difference-between-a-module-and-a-package-in-node-js#
- https://www.quora.com/What-exactly-does-running-JavaScript-inside-a-browser-and-outside-of-a-browser-mean
- https://www.sitepoint.com/understanding-module-exports-exports-node-js/
- https://www.sitepoint.com/beginners-guide-node-package-manager/
- https://www.computerhope.com/jargon/s/server.htm
- https://stackoverflow.com/questions/45171890/what-is-the-syntax-to-export-a-function-from-a-module-in-node-js

