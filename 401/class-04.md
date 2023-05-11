## Data Modeling

Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.


### Reading

#### [nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

##### What type of database is the best fit for the complex query intensive environment?

* SQL databases are a good fit for the complex query intensive environment.

##### What type of database is the best fit for hierarchical data storage?

* Both SQL and NoSQL databases can be a good fit for hierarchical data storage, depending on the specific requirements and use case. SQL databases like PostgreSQL and MySQL support hierarchical data storage through the use of recursive queries, while NoSQL databases like MongoDB and Cassandra can store hierarchical data in nested documents or collections.

##### Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

"Think of a database as a big container where we store lots of information. When we have a lot of data to store, we need to make sure that the database is able to handle all of it and that it can still work quickly and efficiently.

Now, imagine you have a big bookshelf with lots of books on it. If you need to add more books to the shelf, you might run out of space pretty quickly. That's kind of like how a SQL database works. It's like a bookshelf with limited space, and when you start adding more and more data to it, it can become slower and less efficient.

On the other hand, a NoSQL database is more like a filing cabinet with lots of drawers. Each drawer can hold a lot of information, and if you need to add more drawers, you can just keep adding more and more. This makes it easier to handle a lot of data without slowing down.

So, in summary, SQL databases are good for smaller amounts of data that can fit on a "bookshelf," while NoSQL databases are better for larger amounts of data that need to be stored in lots of "drawers" that can be easily expanded as needed." - ChatGPT


#### [sql modeling techniques](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/)

##### Among data tables, what is a one-to-many relationship and how do we “relate” them?
* A one-to-many relationship means an entry in one table can be related to more than one entry in another

##### Prior to designing your relational database, it might be useful to **create**___ a **diagram**___ of the database tables and their relationships.

##### Explain the difference between a primary and foreign key.
* The **primary keys** uniquely identify each row in a table
* The **Foreign Key** is a column or set of columns which match a primary key in another table.
* The match between the foreign key and the primary key is what “glues” the database together.

### Videos

[sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

##### How do we treat keywords and parameters differently in SQL syntax?

"In SQL syntax, keywords and parameters are treated differently in terms of their usage and formatting.

Keywords are reserved words that have specific meanings and functions in the SQL language. They are used to define the structure of a query and to perform operations on the database. Examples of SQL keywords include SELECT, FROM, WHERE, JOIN, and ORDER BY. Keywords are usually written in uppercase letters, although this is not strictly required by the SQL syntax.

Parameters, on the other hand, are values that are passed into a query to produce specific results. They are used to filter, sort, or manipulate the data in the database. Parameters are usually written in lowercase letters, and they are often enclosed in single quotes (') or double quotes (") depending on the database system being used.

In SQL syntax, it is important to distinguish between keywords and parameters to ensure that the query is correctly structured and executed. The SQL engine recognizes keywords and interprets them as instructions, while it treats parameters as data values to be used in the query." - ChatGPT

##### Define normalization within the context of schemas and data.

"Normalization is a process of organizing and structuring data in a database to minimize redundancy and dependency. It involves breaking down a table into smaller, more specialized tables and establishing relationships between them. The goal of normalization is to eliminate data redundancy, reduce data anomalies, and improve data consistency.

Normalization typically involves dividing large tables into smaller ones and defining relationships between them using keys. There are several normal forms, each with its own set of rules that dictate how tables should be structured.

The first normal form (1NF) requires that all data in a table must be atomic, meaning it cannot be further divided into smaller pieces. The second normal form (2NF) requires that each non-key attribute in a table must depend on the entire primary key, not just a part of it. The third normal form (3NF) requires that there should be no transitive dependencies between non-key attributes.

Normalization helps ensure data consistency, accuracy, and integrity, which in turn makes it easier to maintain and update the database. It also reduces the risk of data inconsistencies and errors, which can lead to incorrect results and unreliable data." - ChatGPT

##### Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

"A one-to-one relationship is when one record in a table is associated with only one record in another table, and vice versa. For example, let's say we have a table of employees and a table of Social Security numbers. Each employee has only one Social Security number, and each Social Security number is only associated with one employee. This is an example of a one-to-one relationship.

A one-to-many relationship is when one record in a table is associated with many records in another table, but the records in the other table are associated with only one record in the first table. For example, let's say we have a table of departments and a table of employees. Each department has many employees, but each employee is associated with only one department. This is an example of a one-to-many relationship.

Finally, a many-to-many relationship is when many records in one table are associated with many records in another table. In this case, we need an intermediate table to manage the relationship. For example, let's say we have a table of students and a table of courses. Each student can enroll in many courses, and each course can have many students enrolled. We would need an intermediate table to manage the relationship between students and courses. This is an example of a many-to-many relationship." - ChatGPT

### Bookmark and Review

[sequelize api](https://sequelize.org/docs/v6/)

### Reflection

##### What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-04/)?

These two learning objectives stand out to me: 

* Create models with constraints, relations, type checking, and validity using Sequelize.
* Create an extensible CRUD interface and an implementation for a data model.


## Things I want to know more about

* I am excited to dive in and create various DB schemas, and learn how to maneuver around them. 