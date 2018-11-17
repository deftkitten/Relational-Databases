# Relational-Databases

## Intro  
- **persistent data** - data in database outlives the programs that run on it  
- safe data - hardware failures, software failures, malicious users, etc., want to make sure data remains consistent  
- multi-user - **concurrency control**  
- convenient - powerful and interesting processing, physical data independence - operations on the data is independent from how the data is laid out
  - high level query languages - obey declarative
- efficiency - thousands of queries or updates per second
- reliability - critically important that it’s up all the time

when building database applications, sometimes build with a framework like Django, Ruby on rails
database systems are used in conduction with **middle-ware** - application servers, web servers  

**DBMS** - database management system  

### Key Concepts
- data model - how data is structured
    - relational - set of records
    - XML - heirarhical structure
    - graph - data in form of notes and edges
- schema vs data - kinda like types vs variables, data is stored in the schema
- data definition language (DDL) - setup schema structure for database
- data manipulation language (DML) - querying and modifying

### Key People
- DBMS implementer - builds system
- database designer - establishes schema
- database application developer - programs that operate on the database
- database administrator - loads data, keeps running

## The Relational Model
- underlies all commercial database systems
- very simple model
- efficient implementations

- database - set of relations (or tables)
- each relation has a set of named attributes (or columns)
- actual data itself is stored in the rows (or tuples) in the tables
- each attribute has a type (or domain) - integer, float, jpeg file
- null - special value for unknown or undefined
- key - attribute of a relation where every value is unique (student id, etc.)

creating relations in SQL:  
- basic definition - `Create Table Student(ID, name, GPA, photo)`  
- define types - `Create Table Student(name string, state char(2), ….)`


## Querying Relational Databases
steps in creating and using a relational database:
1. design schema; create using DDL
2. bulk load initial data
3. repeat: execute queries and modifications

Ad-hoc queries in high level language
some queries easy to pose but hard to execute and vice versa
queries return relations (“compositional”, “closed”)
- when you query multiple relations, you get a table in return, this is called closure
compositionally - ability to run a query over the result of our previous query

### Query Languages
relational algebra - formal
SQL - actual / implemented








