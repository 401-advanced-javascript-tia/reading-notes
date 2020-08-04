## July 23<sup>rd</sup>

### Database Normalization

https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/
-*Process used to organize db into tables and columns*
- Limit tables to one purpose
- Reasons for normalizing a database:
  - Minimize duplicate data
  - Minimize/avoid data modification issues
    - Mod anomalies
      - Insert anomaly
      - Update anomaly
      - Delete anomaly
  - Simplify queries

- 3 forms of database normalization (1<sup>st</sup> or 1NF, 2<sup>nd</sup> or 2NF, 3<sup>rd</sup> or 3NF)
  - 1NF: info store in relational table, each column has values. No repeating groups of columns
  - 2NF: table in 1NF and columns depend on primary key
  - 3NF: table in 2NF and all columns not dependent on primary key