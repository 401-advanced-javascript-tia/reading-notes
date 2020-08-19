## Aug 17<sup>th</sup>
## Express

### Express Routing
***
- Event driven system
  - `app.get( '/thing' , (req,res) => {} )`
- Request object can include parameters or query strings
  - `app.get('/api/:thing',...)` = `req.params.thing`
  - `http://server/route?ball=round` = `req.query.ball`
- Response object sends data back to browser
  - has methods that Express uses to format output to browser
    - `send()` and `status()`

### Express Middleware
***
- Series of functions req goes through (invoked by routing layer before request handler is made)
  - definied route, do something first, then pass to next function
  - each receives `request`, `response`, `next` as params
- Application middleware
- Route middleware


### Modularization and Separation of Concerns
***
- Separate code into logical chunks, each doing the thing it rules at
- Dan Abramov: http://react-file-structure.surge.sh/
  - put everything in one file, break it up when that's annoying. then break up more when that's annoying. aaaand etc etc.

### CRUD Operations with REST and Express
***
- CREATE: `app.post('/resource')``
app.post('/resource')
- READ: `app.get('/resource')`
app.get('/resource')
- UPDATE: `app.put('/resource/:id')`
app.put('/resource/:id')
- DESTROY: `app.get('/resource/:id')`


### Server Testing
***
- Can export server as a module in a library to avoid starting *actual* server for testing
  - use `supertest` then to run tests, hits routes as if it were server
  - eliminates variables while testing
  - **(although, wouldn't you want to test server as well? or is this just saying to test it separately from actual production code?)**
- Can also wrap `superagent` in module, then create `__mocks__` folder where this module is, with same-named file in it (named same as module name)
  - invoke `jest.mock()` on file in mocks folder, jest will use mocks version instead of real one
  - **Neat** because you can fake all calls to API (don't want tests to be dependent on API running so mock it like we did on minimist in notesyb)

### Test Pyramid
***
- Server testing
    - Units: Server Internal Functions
      - Mock any integrations (like data fetching)
    - Integration (re connection to other servers)
      - tests for something all the way through, see if it performs through the end
      - Really connect to other services (hard dependencies)
    - Acceptance
      - The server might be a dependency of some other test

### Other New Vocab:
***
- **Curried middleware**: can take a parameter  
- **Higher order function**: function that returns another function, and/or takes another function as an argument

#### Resources
- https://expressjs.com/en/guide/using-middleware.html
- https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm
- https://expressjs.com/en/guide/routing.html
- https://github.com/visionmedia/supertest
- https://expressjs.com/en/resources/middleware.html
- https://www.restapitutorial.com/httpstatuscodes.html
