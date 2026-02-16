## The SQL BETWEEN Operator

The `BETWEEN` operator selects values within a given range. The values can be numbers, text, or dates.

The `BETWEEN` operator is inclusive: begin and end values are included.

## Syntax

SELECT _column name(s)_
FROM _table_name_
WHERE _column name_ BETWEEN _value1_ AND _value2;

### Example

Selects all products with a price between 10 and 20:

SELECT * FROM Products  
WHERE Price BETWEEN 10 AND 20;
## NOT BETWEEN

To display the products outside the range of the previous example, use `NOT BETWEEN`:

### Example

SELECT * FROM Products  
WHERE Price NOT BETWEEN 10 AND 20;
## NOT BETWEEN Text Values

The following SQL statement selects all products with a ProductName not between Carnarvon Tigers and Mozzarella di Giovanni:

### Example

SELECT * FROM Products  
WHERE ProductName NOT BETWEEN 'Carnarvon Tigers' AND 'Mozzarella di Giovanni'  
ORDER BY ProductName;

## BETWEEN Dates

The following SQL statement selects all orders with an OrderDate between '01-July-1996' and '31-July-1996':

### Example

SELECT * FROM Orders  
WHERE Order Date BETWEEN #07/01/1996# AND #07/31/1996#;