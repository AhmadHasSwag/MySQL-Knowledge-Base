## The SQL MIN() and MAX() Functions

The `MIN()` function returns the smallest value of the selected column.

The `MAX()` function returns the largest value of the selected column.

## Syntax

SELECT MIN(_column name_)
FROM _table_name_
WHERE _condition_;`

SELECT MAX(_column name_)
FROM _table_name_
WHERE _condition_;`
### MIN Example
Find the lowest price in the Price column:

SELECT MIN(Price)  
FROM Products;
### MAX Example
Find the highest price in the Price column:

SELECT MAX(Price)  
FROM Products;