## The SQL AVG() Function

The `AVG()` function returns the average value of a numeric column.

## Syntax

SELECT AVG(_column_name_)
FROM _table_name_ 
WHERE _condition_;


### Example

Find the average price of all products:

SELECT AVG(Price)  
FROM Products;