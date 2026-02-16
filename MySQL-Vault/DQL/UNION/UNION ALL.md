## The SQL UNION ALL Operator

The `UNION ALL` operator is used to combine the result-set of two or more `SELECT` statements.

The `UNION ALL` operator includes all rows from each statement, including any duplicates.

Requirements for `UNION ALL`: 

- Every `SELECT` statement within `UNION ALL` must have the same number of columns
- The columns must also have similar data types
- The columns in every `SELECT` statement must also be in the same order

### UNION ALL Syntax

While the `[UNION](https://www.w3schools.com/sql/sql_union.asp)` operator removes duplicate values by default, the `UNION ALL` includes duplicate values:

SELECT _column_name(s)_ FROM _table1_  
UNION ALL  
SELECT _column_name(s)_ FROM _table2_;

**Note:** The column names in the result-set are usually equal to the column names in the first `SELECT` statement.