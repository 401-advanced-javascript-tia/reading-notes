## Aug 12<sup>th</sup>
## Advanced Mongo/Mongoose

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

### 5. Describe how NoSQL Databases scale horizontally.

- Data can easily be split horizontally because of how data is stored. You don't have relations and you can split data in one collection because they're "stand-alone". 

### 6. Give one strong argument for and against NoSQL Databases.

- *For*: super flexible and great when you have data in different formats 
- *Against*: not great when you want to consistenyl update information, since you'd need to update it in all the places it exists. Differs from a SQL db because of the relational nature. 

### 7. Define three related pieces of data in a possible app. (Ex for a store app might be Product, Category, and Department). Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. (For ex, each Product has a Category and belongs in a Department). 

- Gardening app with Users, Plants, and Notes. Each user has a collection of Plants, and each Plant has a collection of Notes. 
- User and Plants would be one-to-many, and the same for Notes to Plants. 

### 8. Name 3 cloud based NoSQL Databases. 

- Atlas: highly-scalable
- DynamoDB: AWS NoSQL Database. Very highly scalable. Also provides a ‘mongoose’-like ORM called ‘dynamoose’
- CosmosDB: Microsoft Azure equivalent


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

- https://dev.to/paulasantamaria/testing-node-js-mongoose-with-an-in-memory-database-32np
- https://cubettech.com/resources/blog/introduction-to-repository-design-pattern/
- https://www.npmjs.com/package/mongodb-memory-server
- https://www.npmjs.com/package/@code-fellows/supergoose
