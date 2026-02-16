## The SQL UNION Operator

The `UNION` operator is used to combine the result-set of two or more `SELECT` statements.

The `UNION` operator automatically removes duplicate rows from the result set.

Requirements for `UNION`:

- Every `SELECT` statement within `UNION` must have the same number of columns
- The columns must also have similar data types
- The columns in every `SELECT` statement must also be in the same order

### UNION Syntax

SELECT _column_name(s)_ FROM _table1_  
UNION  
SELECT _column_name(s)_ FROM _table2_;

**Note:** The column names in the result-set are usually equal to the column names in the first `SELECT` statement.
### Example

Show the year, subject, and name of physics winners for 1980 together with the chemistry winners for 1984.


select * from nobel  where yr = 1980 and subject = 'physics'
UNION 
select * from nobel  where yr = 1984 and subject = 'chemistry'

In this tutorial we will use the well-known Northwind sample database.

Below is a selection from the "Customers" table:

|CustomerID|CustomerName|ContactName|Address|City|PostalCode|Country|
|---|---|---|---|---|---|---|
|1|Alfreds Futterkiste|Maria Anders|Obere Str. 57|Berlin|12209|Germany|
|2|Ana Trujillo Emparedados y helados|Ana Trujillo|Avda. de la Constitución 2222|México D.F.|05021|Mexico|
|3|Antonio Moreno Taquería|Antonio Moreno|Mataderos 2312|México D.F.|05023|Mexico|

And a selection from the "Suppliers" table:

|SupplierID|SupplierName|ContactName|Address|City|PostalCode|Country|
|---|---|---|---|---|---|---|
|1|Exotic Liquid|Charlotte Cooper|49 Gilbert St.|London|EC1 4SD|UK|
|2|New Orleans Cajun Delights|Shelley Burke|P.O. Box 78934|New Orleans|70117|USA|
|3|Grandma Kelly's Homestead|Regina Murphy|707 Oxford Rd.|Ann Arbor|48104|USA|

---

---

## SQL UNION Example

The following SQL statement returns the cities (only distinct values) from both the "Customers" and the "Suppliers" table:

### Example

SELECT City FROM Customers  
UNION  
SELECT City FROM Suppliers  
ORDER BY City;