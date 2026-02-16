## The SQL SELECT TOP Clause

The `SELECT TOP` clause is used to specify the number of records to return.

The `SELECT TOP` clause is useful on large tables with thousands of records. Returning a large number of records can impact performance

- Used in **SQL Server** and **MS Access**.
    
- Placed **right after** `SELECT`.
    
- Can return a **number** or a ==**percentage**== of rows <---------------
## Syntax

SELECT TOP _number_|_percent_ _column_name(s)_  
FROM _table_name  
WHERE _condition_;

### Example

Select only the first 3 records of the Customers table:

SELECT TOP 3 * FROM Customers;