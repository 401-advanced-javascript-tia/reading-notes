## Aug 19<sup>th</sup>
## API Server

### Express - Router Parameters
***
- Can run middleware on a route by adding it like so:
  - `app.get('/products/id', getThing, (req,res) => {`
- Can also run middleware on all routes like so:
  - `app.use(getThing);`
- Both have disadvantages! With Express you can run middleware whem certain params are present

### Sub Documents in Mongoose
***
- *Mongoose is schema-driven ORM, brings structure to Mongo docs*
- Can nest documents (helpful when a document contains a list of other documents)
- Can declare shared schema, but then we have to connect the data and "populate" it
  - Even if shared, still need to update single piece of info across areas it lives


### Joining Data/Documents in Mongo
***
- *Note that noSQL Databases don’t really join, and doing so generally is considered an anti-pattern. Ensure that you’re modeling things in the most logical way for this data store.*
- Mongoose method `populate()` connects 2 collections
  - 1: physically joining by using a reference to another collection
  - 2: virtual population: create virtual field in a doc pointed to a field in another one. Use `pre('find')` can make collection on the fly (more efficient than storing the relation)

### Virtual Joins
***
- Can define more sophisticated relationships between documents

### Resources
- https://expressjs.com/en/4x/api.html#router.param
- https://mongoosejs.com/docs/middleware.html
- https://mongoosejs.com/docs/subdocs.html
- https://mongoosejs.com/docs/populate.html#populate-virtuals
