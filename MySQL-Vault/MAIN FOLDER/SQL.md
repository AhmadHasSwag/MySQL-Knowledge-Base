SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users to query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

## What Can SQL do?

- SQL can execute queries against a database
- SQL can retrieve data from a database
- SQL can insert records in a database
- SQL can update records in a database
- SQL can delete records from a database
- SQL can create new databases
- SQL can create new tables in a database
- SQL can create stored procedures in a database
- SQL can create views in a database
- SQL can set permissions on tables, procedures, and views

## Using SQL in Your Web Site

To build a web site that shows data from a database, you will need:

- An ==**RDBMS**== (Relational Database Management System )database program (i.e. MS Access, SQL Server, My-SQL)
- To use a server-side scripting language, like PHP or ASP
- To use SQL to get the data you want
- To use HTML / CSS to style the page

##  SQL Command Categories

[[DQL(Data Query Language)]]
- Server, My-SQL
- To use a server-side scripting language, like PHP or ASP
- To use SQL to get the data you want
- To use HTML / CSS to style the page
- Commands
	- select
 [[DML (Data Manipulation Language)]]
- DML commands are used to manipulate the data stored in database tables.
- With DML, you can insert new records
- update existing ones, delete unwanted data or retrieve information.
- Commands :
	- update
	- insert into
	- Delete
[[DCL (Data Control Language)]]
- These commands manage **permissions and access control**.
- Common DCL commands:
	- `GRANT` – give privileges
	- `REVOKE` – remove privileges
- Purpose:  Security and user rights.
[[TCL (Transaction Control Language)]]
- Used to manage **transactions** and ensure data integrity.
- Commands
	- `COMMIT`
	- `ROLLBACK`
	- `SAVEPOINT`
	- `SET TRANSACTION`    
- Purpose: Control how changes are saved or undone.
[[DDL (Data Definition Language)]]
-  define and modify database structure (schemas, tables, indexes). 
- Commands
	- CREATE
	- ALTER
	- DROP
	- TRUNCATE. 
- Key point:  DDL changes the _schema_ not the row-level content; 
- many DDL operations are DDL-level metadata changes that may require privileges and can be destructive

### LINKS

[[Administrative Command]]