## Readings: MongoDB and Mongoose

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

Fill in the chart below with five differences between SQL and NoSQL databases:

        SQL                     	NoSQL
 Relational Databases     |    Non-relational, or distributed
------------------------------------------------------------
 table based               |  document based, key-value pairs
-------------------------------------------------------------
 represent data in         |        do not have standard 
 form of tables	           |         schema definitions
 ------------------------------------------------------------
 predefined schema         |    dynamic schema, unstructured data
 ------------------------------------------------------------
 vertically scalable       |    horizontally scalable
 ------------------------------------------------------------
 SQL                       |           UnSQL
(Structured query language)   (Unstructured Query Language)
------------------------------------------------------------
* For complex queries:
 Good fit for complex      |        Not a good fit
 Querys of large data      |      for complex querys
 ------------------------------------------------------------
 * For the type of data to be stored:
 Not best fit for          |      better fit due to
 hierarchical data storage |     key value pair storage
 ------------------------------------------------------------
                             |  preferred for large data
------------------------------------------------------------
* For scalability: 
vertically scalable         |   horizontally scalable
------------------------------------------------------------
* For high transactional based application: 
best fit for heavy          |
duty transactional          |    
------------------------------------------------------------
* For support:
Excellent support available |    community support
------------------------------------------------------------
* For properties:
ACID properties             |          CAP theorem    
Atomicity, Consistency,     |    Consistency, Availability
Isolation Durability)       |     and Partition tolerance 
------------------------------------------------------------
* For DB types:
either open-source or       |      graph, key-value
close-sourced               |  document, column  and XML .
------------------------------------------------------------

 	 
#### What kind of data is a good fit for an SQL database?
Give a real world example.
Credit Card transactions at a store. They need security and support and need to be able to handle high traffic
Give a real world example.

#### What kind of data is a good fit a NoSQL database?
Give a real world example.
Start up business. Needs flexibility and room for growth. 


#### Which type of database is best for hierarchical data storage?
UnSQL due to key value pair storage

#### Which type of database is best for scalability?
If you need vertical scalability: SQL
If you need horizontal scalability: UnSQL

### Videos
### [sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

#### What does SQL stand for?
 structured query language

#### What is a relational database?
"It means we have a database which
works with certain assumptions or in a
certain way"

#### What type of structure does a relational database work with?
Tables, 
#### What is a ‘schema’?
"a representation of a plan or theory in the form of an outline or model."

#### What is a NoSQL database?
"aka "not only SQL") are non-tabular databases and store data differently than relational tables"

#### How does it work?
"NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads."-MongoDB



#### What is inside of a MongoDB database?
MongoDB derived from the work humongous is built to store lots and lots of data in a very efficient way. 
It has collections that you could translate with tables essentially and it looks a bit like JSON.

#### Which is more flexible - SQL or MongoDB? and why.
Mongo- it can use a variety of Schema to store data
"Non-relational databases are most suited to handling large volumes of data and/or unstructured data. They’re extremely popular in the world of big data because writes are fast. NoSQL databases don’t enforce complicated cross-table schemas, so writes are unlikely to be a bottleneck in a system using NoSQL."

#### What is the disadvantage of a NoSQL database?
Less Secure
Cannot handle high traffic as well. 

### Bookmark and Review
mongoose api
React Router

#### How does this subject matter as it relates to what I am studying?
We are about to start a project that utilizes MongoDB

#### Things I want to know more about:

Also see: [Five Common Data Stores and When to Use Them](https://shopify.engineering/five-common-data-stores-usage)