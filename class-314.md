## [Database Normalization (Explained in Simple English)](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

### Introduction

*Database Normalization* is a process used to organize a database into tables and columns
  - By limiting a table to one purpose you reduce the number of duplicate data contained in the database

### Reasons for Database Normalization

1. Minimize Duplicate Data
1. Minimize Data Modification Issues
1. Simplify Queries

### Data Duplication and Modification Anomalies

Duplicated information can present problems such as:
- Increased storage / Decreased performance
- It becomes more difficult to maintain data changes

Modification anomalies include:
- Insert Anomaly (missing data when creating new rows)
- Update Anomaly (inconsistancies in data should an update not include some necessary rows)
- Deletion Anomaly (deleting a row may remove more data than intended if rows serve multiple purposes)

### Search and Sort Issues

- Database Normalization makes it easier to search and sort your data reliably

### Definition of Database Normalization

**1NF**: Information is stored in a relational table with each column containing atomic values.  No repeating groups of columns

**2NF**: Table is in 1NF AND all columns depend on the table's primary key

**3NF**: Table is in 2NF AND all columns are not transitively dependent on the primary key

---

[Home](https://jchinzi.github.io/reading-notes/)