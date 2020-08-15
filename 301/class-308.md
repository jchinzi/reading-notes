## [SQLBolt](http://sqlbolt.com/)

SQLBolt is an interactive teaching tool to introduce users to SQL.  Below, I've compiled notes taken during the provided exercises:

### SELECT queries 101

- SELECT statements are used to retrieve data from a SQL database

- SQL tables contain many instances of a particular type of thing which may share traits

The syntax used is 
>SELECT ***column*** FROM ***table***;

### Queries with constraints

- ***WHERE*** clause can be used in the query to filter certain results from being returned

>SELECT ***column*** FROM ***table*** WHERE ***condition***;

### Filtering and sorting Query results

- ***DISTINCT*** keyword will remove duplicate rows

>SELECT DISTINCT ***column*** FROM ***table*** WHERE ***condition***;

-***ORDER BY*** allows us to sort rows alpha-numerically, ascending or descending

>SELECT ***column*** FROM ***table*** WHERE ***condition*** ORDER BY ***column*** ASC/DESC;

- ***LIMIT*** will reduce the number or rows to return

- ***OFFSET*** will specify where to begin counting the number rows from

### Inserting rows

*Database Schema* describes the structure of each table, and the datatypes that each column of the table can contain

***INSERT*** statements are used to insert data into the database:

>   INSERT INTO ***table*** VALUES ***(value)***

### Updating rows

***UPDATE***  can be used to update existing data - the data must match the data type of the columns in the table schema

> UPDATE ***table*** SET ***column = value*** WHERE ***condition***;

- Good practice dictates you test constraints with a SELECT query before writing and UPDATE to prevent errors

### Deleting rows

***DELETE*** statement can be used to delete rows:

> DELETE FROM ***table*** WHERE ***condition***;

### Creating tables

***CREATE TABLE*** statement can be used to create a new database table

>CREATE TABLE IF NOT EXISTS ***table***(**column** *DataType* *TableConstraint* DEFAULT *default_value*);

### Altering tables

***ALTER TABLE***  statement allows you to add, remove, or modify columns and table constraints

- ***ADD, DROP, & RENAME TO***  are all examples of alterations that can be made

> ALTER TABLE ***table*** RENAME TO ***newTableName***;

### Dropping tables

***DROP TABLE*** removes the entire table including all of its data and metadata

> DROP TABLE IF EXISTS ***table***;

---
[Home](https://jchinzi.github.io/reading-notes/)