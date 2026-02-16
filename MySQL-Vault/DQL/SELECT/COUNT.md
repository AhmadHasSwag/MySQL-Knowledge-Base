## The SQL COUNT() Function

The `COUNT()` function returns the number of rows that matches a specified criterion.

## Syntax

SELECT COUNT(_column_name_)
FROM _table_name_ 
WHERE _condition_;

### Example

Find the total number of rows in the `Products` table:

SELECT COUNT (table name)  
FROM Products;

## Specify Column

You can specify a column name instead of the asterix symbol `(*)`.
If you specify a column name instead of `(*)`, NULL values will not be counted.<==================

## Ignore Duplicates

You can ignore duplicates by using the `DISTINCT` keyword in the `COUNT()` function.

If `DISTINCT` is specified, rows with the same value for the specified column will be counted as one.

### Example

How many _different_ prices are there in the `Products` table:

SELECT COUNT(DISTINCT Price)  
FROM Products;
