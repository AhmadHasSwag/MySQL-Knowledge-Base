## The SQL HAVING Clause

The `HAVING` clause was added to SQL because the `WHERE` keyword cannot be used with aggregate functions.

### HAVING Syntax

SELECT _column_name(s)_  
FROM _table_name_  
WHERE _condition_  
GROUP BY _column_name(s)  
_HAVING _condition  
_ORDER BY _column_name(s);_

## SQL HAVING Examples

The following SQL statement lists the number of customers in each country. Only include countries with more than 5 customers:

### Example

SELECT COUNT(CustomerID), Country  
FROM Customers  
GROUP BY Country  
HAVING COUNT(CustomerID) > 5;