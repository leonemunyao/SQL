DATABASE

Data can be facts related to any object inconsideration. Database Management system is a collection of programs which enable its users to database, manipulate data and help in representation of data.

Databases are for storing data. Storing data in your application has the obvious shortcoming that, whatever the technology you are using your data dies when your server stops. A solid database is expected to be acid. Which means it guarantees;

Atomicity - transactions are atomic which means if a transaction fails, the result will be like it never happened.

Consistency - you can define rules for your data and expect the data abides by the rules or the transaction fails. 

Isolation - run two operations at the same time and you can expect that the result is as though they were ran after the other.

Durability - unplug your server at any time, boot it back up and it doesn't loose data. 

ACID is a cool acronym.  CRUD is another cool one


2+ Kinds of DATABASES

When people talk about databases, they are usually referring to Relational Databases(such a PostgreSQL, MySQL, Oracle.). There are many other kinds of databases which are globally referred to as NoSQL Databases. 

SQL

In order to work with relational databases, you will need to get familiar with SQL. 

Engineers that are comfortable with SQL are very respected in the industry.

Terminologies around relational databases.
Say you need to store users. To do that you create a table that is called "users". Your users have three pieces of information to store, their id, their login and their password. Those are called "columns". They all have types like integer for id, vachar[32] for login(a string variable), and a char(32) (a string exactly 32 characters)

Why are they called relational databases. 
Relations -  they gather a lot data related to each other since they follow the same structure. Relation todays refers to something that ties two records together.


A NoSQL kind of database: document-based databases
One popular type of NoSQL database is document oriented databases, such as MongoDB or CouchDB

MySQL

Introduction to MySQL
MySQL is an open source database management system, commonly installed as part of the popular LAMP.(Linux, Apache, MySQL, PHP/Python/Perl). It implements the relational model and uses Structured Query Language(SQL) to manage its data. 

Installing MySQL.
On Ubuntu you can install MySQL using the APT package repository. To install update the package index on the server. Then install <mysql-server> package. 

Configuration of MySQL
For fresh installation of MySQL, you will want to run the DBMS's included security script 


Basic SQL Statements: DDL and DML

SQL Statements are divided into two major categories: data definition language(DDL) and Data Manipulation language. Both of these categories contain far more statements. 

DDL
They are used to build and modify the structure of the tables and other objects in the database. We have the following;

CREATE TABLE - does exactly that
ALTER TABLE - specify foreign and primary key constraints as well as make modifications to the table.
If you totally mess things up and want to start over, you can always get rid of any object you have created with a drop statement. 

DML
They are used to work with data in the tables. They incude;
INSERT INTO - add a new row to a table. 
UPDATE - change values that are already in the table.
DELETE FROM - deletes statememts from the taabe.
COMMIT - if you are using a multi-user system, you may make your DML changes visible to the rest of the users of the databases
ROLLBACK - used if you messed up with the changees in the system.

Basic queries: SQL and RA
Once we have created tables.