## Aug 11<sup>th</sup>
## Data Modeling & NoSQL Databases

### 1. Why would a developer choose to make data models?

- Heaps of benefits to making data models! One big one is that it allows you to see the architecture of an app all the way through and to better define the problem. 

### 2. What purpose do CRUD operations serve?

- These are the four basic functions of persistent storage:
  - **C**reate
  - **R**ead
  - **U**pdate
  - **D**elete

### 3. What kind of database is Postgres? What kind of db is MongoDB?

- Postgres is a SQL (relational) database and MongoDb is a NoSQL database. 

### 4. What is Mongoose and why do we need it?

- Mongoose is an ODM library (I also saw it referred to as an Object Document Mapper) and it allows us to write JavaScript code to interact with our database. With it we can make the connection with our MongoDB and provides shcema-based solution to model the app data. Makes development fast!

### 5. Define three related pieces of data in a possible app. (Ex for a store app might be Product, Category, and Department). Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. (For ex, each Product has a Category and belongs in a Department). 

- Gardening app with Users, Plants, and Notes. Each user has a collection of Plants, and each Plant has a collection of Notes. 
- User and Plants would be one-to-many, and the same for Notes to Plants. 


### Vocabulary

| **Term**      | **Definition** |
| ------------- | -------------- |
| **database** | works with tables that are essentially "data bins" or storage containers   |
| **data model** | a model that organizes elements of data and how they all relate to one another |
| **CRUD** | Create, Read, Update, Delete  |
| **schema** | says which data can go into a table, defined by certain fields |
| **sanitize** | to check a piece of user input before storing it in a database  |
| **Structured Query Language (SQL)** | language that allows you to write database queries. uses keywords, specific syntax. and our data and parameters. characterized by a strong schema and the relational nature of the data |
| **Non SQL (NoSQL)** | database that uses collections instead of tables. documents in the collections (similar to rows in tables in SQL) but interesting thing is they dont have to use schema. in general, no relations in a NoSQL world. put all information in one place. less relation merging means super fast queries. |
| **MongoDB** | a NoSQL database. stores heaps of data in an efficient way which might be why its so popular!  |
| **Mongoose** | Object Data Modeling (ODM) library for MongoDB and Node. manages relationships between data, translates objects in code and representations of those in Mongo|
| **record** | in SQL db. a row in a table, a new entry that has values for the fields we defined in the schema |
| **document** | in NoSQL db, its what a collection is comprised of (similar to rows in table)      |
| **Object Relation Mapping (ORM)** | technique of accessing a relational database using an object-oriented language (JavaScript, in our case!), "a way to manage database data by mapping database tables to classes and instances of classes to rows in those tables"  |


#### Rescouces

- vid: www.youtube.com/watch?v=ZS_kXvOeQ5Y
- https://en.wikipedia.org/wiki/Data_model
- https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/
- https://medium.com/@tamires.lowande/orms-in-js-vs-ruby-3908b6b8893f
- https://www.quora.com/What-is-Mongoose

*Cloud Databases*
*There are a few alternatives to running Mongo locally for your web servers*

*MLab - remotely hosted mongoDB systems. Easily setup a free database (or pay for more horsepower). Works great with Heroku*
*Atlas - Cloud based, highly scalable Mongo DB*
*DynamoDB - AWS NoSQL Database. Very highly scalable. Also provides a ‘mongoose’-like ORM called ‘dynamoose’*
*CosmosDB - The Microsoft Azure equivalent for Atlas and Dynamo*


### Notes from lecture Tues 08-12-2020

- "NoSQL" could also mean "not only SQL", not just "no"
- SQL is good for structured data
- NoSQL is good for document-based databases (just collect a bunch of info and store it somewhere) 
- ODM = Object Document Modeler