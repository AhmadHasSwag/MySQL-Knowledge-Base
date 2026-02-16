The `ANY`  operator allow you to perform a comparison between a single column value and a range of other values.
## The SQL ALL Operator

The `ALL` operator:

- returns a boolean value as a result
- returns TRUE if ALL of the subquery values meet the condition
- is used with `SELECT`, `WHERE` and `HAVING` statements

`ALL` means that the condition will be true only if the operation is true for all values in the range. 

### ALL Syntax With SELECT

SELECT ALL _column_name(s)_  
FROM _table_name_  
WHERE _condition_;

### ALL Syntax With WHERE or HAVING

SELECT _column_name(s)_  
FROM _table_name_  
WHERE _column_name operator_ ALL  
(SELECT _column_name_  FROM _table_name_  WHERE _condition_);


### Example

The following SQL statement lists the ProductName if ALL the records in the OrderDetails table has Quantity equal to 10. This will of course return FALSE because the Quantity column has many different values (not only the value of 10):

SELECT ProductName  
FROM Products  
WHERE ProductID = ALL  
	 (SELECT ProductID  
	  FROM OrderDetails  
	  WHERE Quantity = 10);