## IN Operator

The `IN` operator allows you to specify multiple values in a `WHERE` clause.

The `IN` operator is a shorthand for multiple `OR` conditions.

## Syntax

SELECT _column name(s)_
FROM _table_name_ 
WHERE _column name_ ==**IN**== (_value1_, _value2_, ...);

## IN (SELECT)

You can also use `IN` with a subquery in the `WHERE` clause.

With a subquery you can return all records from the main query that are present in the result of the subquery.

### Example

Return all customers that have an order in the Orders table:

SELECT *
FROM Customers  
WHERE CustomerID IN (SELECT CustomerID FROM Orders);

## NOT IN (SELECT)

The result in the example above returned 74 records, that means that there are 17 customers that haven't placed any orders.

Let us check if that is correct, by using the `NOT IN` operator.

### Example

Return all customers that have NOT placed any orders in the orders table:

SELECT * 
FROM Customers  
WHERE CustomerID NOT IN (SELECT CustomerID FROM Orders);