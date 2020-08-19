## Aug 18<sup>th</sup>
## Express Routing & Connected API

### Route Modularization
***
- index.js - Entry Point
- server.js - Hub, Exported Server
- models/categories.js, etc - Data Models
- routes/categories.js, etc - Routers and Handlers

### Routing
***
- *Reminder*
  - `const express = require('express')`
  - `const app = express();`
- app.use to specify middleware as callback function (or "handler" function)
- **order you place middleware and routes is super important!**
  - everything happens in order it appears

- **Methods**
  - app.get
  - app.post
  - app.put
  - app.delete
  - app.all loads middleware for all methods to that route

-**Paths**
  - route paths with request method define endpoints where req is made
  - query strings *not* part of route path
  - can be strings, string patterns, regex
    - string pattern ex: `app.get('/ab*cd', function(req,res)...` will match abxcd, abRANDOMcd, ab123cd, etc

- **Route Params**
`Route path: /users/:userId/books/:bookId`
`Request URL: http://localhost:3000/users/34/books/8989`
`req.params: { "userId": "34", "bookId": "8989" }`
***
`app.get('/users/:userId/books/:bookId', function (req, res) {`
   `res.send(req.params)  `
`})`
- more than one callback can handle a route, but need to pass in next param
- even an array of functions could handle a route, or a combo of arr and independent function:
`app.get('/example/d', [cb0, cb1], function (req, res, next) {`
  `console.log('the response will be sent by the next function ...')`
  `next()`
`}, function (req, res) {`
  `res.send('Hello from D!')`
`})`

- **Response Methods**

| Method | Description|
| ------ | ---------- |
| res.download() |	Prompt a file to be downloaded. |
| res.end() |	End the response process. |
| res.json() |	Send a JSON response. |
| res.jsonp() |	Send a JSON response with JSONP support. |
| res.redirect() |	Redirect a request. |
| res.render() |	Render a view template. |
| res.send() |	Send a response of various types. |
| res.sendFile() |	Send a file as an octet stream. |
| res.sendStatus() |	Set the response status code and send its string representation as the response body. |

- **app.route()**
  - create chainable route handlers
  - use express.Router
- can define multiple actions on a route
`app.route('/login')`
  `.get(function(req,res) {res.send ('this is login form') })`
  `.post(function(req,res) {console.log('processing')...`

## Express Router
- New feature of Express 4.0, mini Express app with *just* the routing stuff
- Provides routing APIs (.use, get, .param)
`const router = express.Router()`
`router.get('/', function...)`
`app.use('/', router)`
- Can create multiple routers- maybe one for basic routes, one for API routes, one for authenticated routes

- **Route Middleware for Params**
  - `.param()` creates middleware that runs for certain route parameter
  - Can be used to validate data coming to app (like a token for the RESTful API)
### Resources
- https://expressjs.com/en/guide/routing.html
- https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4
