## The SQL ANY  Operators

The `ANY`  operator allow you to perform a comparison between a single column value and a range of other values.

---

## The SQL ANY Operator

The `ANY` operator:

- returns a boolean value as a result
- returns TRUE if ANY of the subquery values meet the condition

`ANY` means that the condition will be true if the operation is true for any of the values in the range.

### ANY Syntax

SELECT _column_name(s)_  
FROM _table_name_  
WHERE _column_name operator_ ANY  
(SELECT _column_name_  FROM _table_name_  WHERE _condition_);

## SQL ANY Examples

The following SQL statement lists the ProductName if it finds ANY records in the OrderDetails table has Quantity equal to 10 (this will return TRUE because the Quantity column has some values of 10):

### Example

SELECT ProductName  
FROM Products  
WHERE ProductID = ANY  
  (SELECT ProductID  
  FROM OrderDetails  
  WHERE Quantity = 10);