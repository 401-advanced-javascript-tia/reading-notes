## July 12<sup>th</sup>

### Node, Express, APIs
https://www.sitepoint.com/an-introduction-to-node-js/
- Includes installation directions!

**Node is an environment that allows us to write JavaScript in the backend**
- Built on Google Chrome's V8 JavaScript Engine
  - V8 is the open-source JavaScript engine that runs in Chrome
  - Program we can use to execute JavaScript on our computers (a js runtime)

- **npm** is the package manager that comes bundled with Node
  - "npm -v" tp find what version is installed
  - https://www.sitepoint.com/beginners-guide-node-package-manager/

- Node and npm are designed to automate the process of developing a modern JavaScript app 

- **Node.js lets us run JavaScript on the server**
  - Node is *single-threaded* and *event-driven*- everything that happens in Node is in reaction to an event
    - server starts processing new request, if it encounters a blocking I/O, instead of waiting for it to complete, it registers callback before continuing to process next event
    - I/O operation finises, server executes callback and continues on original request
    - Node uses libuv library to do this async behavior
  - Node can handle large # of simultaneuous connections
  - Node is suited well to apps requiring some form of real-time interaction (chat sites, https://codeshare.io/, building APIs handling I/O driven requests)

- **Major advantages**
  - speed and scalability
  - can easily share code between server and client in same language
  - speaks JSON (most important data exchange format on the Web)
  - can also be used as scripting language
  - write own CLI

  **"Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library."**