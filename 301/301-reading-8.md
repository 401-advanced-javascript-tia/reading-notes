## July 15<sup>th</sup>

### SQL - Structured Query Language

https://sqlbolt.com/
- Language that allows technical and non-technical users to query, manipulate, transform data from db
  - **Relational database** is collection of related (2D) tables
- Safe and scalable storage for websites and mobile apps
- Postgres is SQL db

#### **SELECT queries**
- To retireve data from SQL db
- What we're looking for, how to return it
  - SELECT column, column_two, ...   (or can use * to get everything back to inspect table)
  - FROM mytable;

#### **Query Constraints**
- Can put a **WHERE** clause in the query to filter results
- All strings must be quoted

#### **Filtering and Sorting Results**
- Can discard with **DISTINCT** (blindly removes dup rows)
- **ORDER BY** sorts asc or desc
- **LIMIT** and **OFFSET** indicates the subset you care about

#### **Schemas**
- What describes the structure of the table and datatypes that each column can contain
- **INSERT** declares one or more rows to insert and where


#### *Notes from lecture*

- SQL is **not** a db (Postgres is), it is a language
- Everytime you put something in db, you get an id
- SQL can **SELECT**, **INSERT**, **UPDATE**, **DELETE**
  - What we want to do
  - What columns at play
  - From what table
  - Filtered how
- Make SQL keywords capitals for easy reading
- Do not label columns using camelCase (youll get bugs)
- **Must** use semicolons to end the query (or else SQL will wait for you)
- **INSERT INTO** name of table (column, column), **VALUES** (value, value)
  - Youll get error message if number of values doesnt match number columns
- Postgres is server running on our machine (address 5432)
- **Never** put anything directly into SQL, use $1, $2, etc and make let safeValues

Great cheat sheet here: http://www.cheat-sheets.org/sites/sql.su/