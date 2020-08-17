## Aug 16<sup>th</sup>
## HTTP & REST

### HTTP
***
- *Hyper Text Transfer Protocol* is a "stateless request-response application layer protocol
- Foundation of the web
- Client-server computing model - server is a service-providing host, clients make requests to host
  - HTTP specs define how req and resp are formatted
- Serves `.html` files but also used to xfer img, vid, `.json`, `.xml`, binary executables (program an operating system can run), etc

**Resources**
- https://tools.ietf.org/html/rfc7231


### HTTP Requests
***
- In text and formatted using **TCP** (Transmission Control Protocol)
  - First line: `METHOD`, `URL`, `HTTP VERSION`
  - Following lines: request `HEADERS`
    - key value pair separated with :, more than one value separated with ;

- **Idempotence**: property of certain operations where they can be applied multiple times without changing result beyond initial application
  - Clients can make same call repeatdely while producing same result (making multiple idential requests results in same thing as one single request)
  - two identical requests made they should get identical response
- **Safe** methods only for info retrieval, shouldn't change server state
- If **cachable** client should be able to catch response

| **HTTP Method** | **Request Has Body** | **Response Has Body** | **Safe** | **Idempotent** | **Cacheable** | **Function** |
| --------------- | -------------------- | --------------------- | -------- | -------------- | ------------- | ------------ |
| GET             | No                   | Yes                   | Yes      | Yes            | Yes           | Retrieve a resource |
| HEAD            | No                   | No, see function      | Yes      | Yes            | Yes           | Like GET but headers only |
| POST            | Yes                  | Yes                   | No       | No             | Yes           | Create a resource   |
| PUT             | Yes                  | Yes                   | No       | Yes            | No            | Update a resource |
| DELETE          | No                   | Yes                   | No       | Yes            | No            | Delete a resource |
| CONNECT         | Yes                  | Yes                   | No       | No             | No            | Create TCP/IP tunnel |
| OPTIONS         | Optional             | Yes                   | Yes      | Yes            | No            | Returns supported methods for a URL |
| TRACE           | No                   | Yes                   | Yes      | Yes            | No            | Echos retrieved request |
| PATCH           | Yes                  | Yes                   | No       | No             | No            | Partial modification of resource |


### HTTP Response
***
- Also text, transferred with TCP
  - First line: `HTTP VERSION`, `STATUS CODE`, `STATUS MESSAGE`
  - Following lines: request headers, formatted like request headers

### REST
***
- **RE**presentational **S**tate **T**ransfer - by which we can reference, manipulate, and transfer state
- **API** is Application Program Interface
  - contract provided by one piece of software to another piece of software
  - structured request, structured response
- **API** is the messenger, **REST** lets us use HTTP to format those messages 
- Uses methods (verbs) to operate on state of resource (noun)
- Since it operates using just HTTP and delivers usually in JSON, it can be used by almost any language
- **URI** is Uniform Resource Identifier
   - RESTful endpoint is URI that identifies resource
   - Usually delivers data in JSON format
   - ex: `http://api.server.com/api/v1/people`
    - `http://` is protocol/scheme
    - `api.server.com` is domain or server
    - `/api/v1` is API endpoint
    - `/people` the resource or collection
    - `/people/1234` would be a more specific resource, person with id for ex

| **REST Method** | **CRUD Operation** | **Function** |
| --------------- | ------------------ | ------------ |
| GET             | READ               | Retrieve 1 or more records |
| POST            | CREATE             | Create a new record |
| PUT             | UPDATE             | Update a record through replacement (put it back) |
| PATCH           | UPDATE             | Update a record (just the parts that changed) |
| DESTROY         | DELETE             | Remove a record |

### REST Documentation (Swagger)
***
- Standard in documenting REST APIs is live documentation system through Open API (used to be Swagger)
  - Documentation that allows for live requests from within it. Cool!
  




