# Database Logic & SQL Basics

## Relational Database
### Relational database is a system that organizing data that has logical relationships with each other by representing them in tables (rows and coloumns). Relations between in data is built on common areas of tables. This structure prevents data duplication (normalization) and raises data stability.

## Primary Key & Foreign Key
### Primary Key: A column that uniquely identifies every record in a table. It cannot be 'NULL' and cannot contain duplicate values (e.g. Student number).
### Foreign Key: It keeps the relation between data physically. A data in a table links to another data inthe table. Actually, it is the referencing of a table's Primary Key in another table as a reference.

## Basic SQL Commands
### SELECT: It determines which data will be retrieved from tables in database. It is used with filtration (WHERE) and ordering (ORDER BY).
### JOIN: It combines rows from two or more tables that have relation between joining on common field (generally Foreign Key) 
### GROUP BY: It seperates data groups to specific criteiron. Generally it is used for SUM, COUNT or (average) AVG processes. (e.g. find student number to the cities)

## Index Mechanism and Efficiency
### It provides to access the data in database faster without changing the physical order. It is such a contents field in the book; instead of scanning the whole book it provides the relevant page directly.
### It significantly increases reading speed (SELECT) while making slower writing processes (INSERT/UPDATE) due to updating index list.