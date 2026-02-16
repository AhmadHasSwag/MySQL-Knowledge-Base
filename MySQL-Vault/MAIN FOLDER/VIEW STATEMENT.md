## CREATE VIEW Statement

In SQL, a view is a virtual table based on the result-set of an SQL statement.

A view contains rows and columns, just like a real table. The fields in a view are fields from one or more real tables in the database.

You can add SQL statements and functions to a view and present the data as if the data were coming from one single table.

A view is created with the `CREATE VIEW` statement. 

### CREATE VIEW Syntax

CREATE VIEW _view_name_ AS  
SELECT _column1_, _column2_, ...  
FROM _table_name_  
WHERE _condition_;

**Note:** A view always shows up-to-date data! The database engine recreates the view, every time a user queries it.

---

## SQL CREATE VIEW Examples

The following SQL creates a view that shows all customers from Brazil:

### Example[Get your own SQL Server](https://www.w3schools.com/sql/sql_server.asp "W3Schools Spaces")

CREATE VIEW [Brazil Customers] AS  
SELECT CustomerName, ContactName  
FROM Customers  
WHERE Country = 'Brazil';

We can query the view above as follows:

### Example

SELECT * FROM [Brazil Customers];

The following SQL creates a view that selects every product in the "Products" table with a price higher than the average price:

### Example

CREATE VIEW [Products Above Average Price] AS  
SELECT ProductName, Price  
FROM Products  
WHERE Price > (SELECT AVG(Price) FROM Products);

We can query the view above as follows:

### Example

SELECT * FROM [Products Above Average Price];

---

---

## SQL Updating a View

A view can be updated with the `CREATE OR REPLACE VIEW` statement.

### SQL CREATE OR REPLACE VIEW Syntax

CREATE OR REPLACE VIEW _view_name_ AS  
SELECT _column1_, _column2_, ...  
FROM _table_name_  
WHERE _condition_;

The following SQL adds the "City" column to the "Brazil Customers" view:

### Example

CREATE OR REPLACE VIEW [Brazil Customers] AS  
SELECT CustomerName, ContactName, City  
FROM Customers  
WHERE Country = 'Brazil';

---

## SQL Dropping a View

A view is deleted with the `DROP VIEW` statement.

### SQL DROP VIEW Syntax

DROP VIEW _view_name_;

The following SQL drops the "Brazil Customers" view:

### Example

DROP VIEW [Brazil Customers];