he `SELECT INTO` statement copies data from one table into a new table.

### SELECT INTO Syntax

Copy all columns into a new table:

SELECT *  
INTO _newtable_ [IN _externaldb_]  
FROM _oldtable  
_WHERE _condition_;

Copy only some columns into a new table:

SELECT _column1_, _column2_, _column3_, ...  
INTO _newtable_ [IN _externaldb_]  
FROM _oldtable  
_WHERE _condition;_

The new table will be created with the column-names and types as defined in the old table. You can create new column names using the `AS` clause.

---

## SQL SELECT INTO Examples

The following SQL statement creates a backup copy of Customers:

SELECT * INTO CustomersBackup2017  
FROM Customers;

## The following SQL statement uses the `IN` clause to copy the table into a new table in another database:


SELECT * INTO CustomersBackup2017 IN 'Backup.mdb'  
FROM Customers;

## The following SQL statement copies only a few columns into a new table:

SELECT CustomerName, ContactName INTO CustomersBackup2017  
FROM Customers;

## The following SQL statement copies data from more than one table into a new table:

SELECT Customers.CustomerName, Orders.OrderID  
INTO CustomersOrderBackup2017  
FROM Customers  
LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID;

### LINKS

[[DML (Data Manipulation Language)]]