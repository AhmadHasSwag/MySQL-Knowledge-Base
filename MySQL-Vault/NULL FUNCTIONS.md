## SQL IFNULL(),  COALESCE(), Functions

Look at the following "Products" table:

|P_Id|ProductName|UnitPrice|UnitsInStock|UnitsOnOrder|
|---|---|---|---|---|
|1|Jarlsberg|10.45|16|15|
|2|Mascarpone|32.56|23||
|3|Gorgonzola|15.67|9|20|

Suppose that the "UnitsOnOrder" column is optional, and may contain NULL values.

Look at the following SELECT statement:

SELECT ProductName, UnitPrice * (UnitsInStock + UnitsOnOrder)  
FROM Products;

In the example above, if any of the "UnitsOnOrder" values are NULL, the result will be NULL.

---

## Solutions

**MySQL**
## [IFNULL()]
 lets you return an alternative value if an expression is NULL:
## Syntax
SELECT IFNULL (OLD VARIABLE,NEW VARIABLE)
FROM TABLE


SELECT ProductName, UnitPrice * (UnitsInStock + IFNULL(UnitsOnOrder, 0))  
FROM Products;
