## The SQL INSERT INTO SELECT Statement

The `INSERT INTO SELECT` statement copies data from one table and inserts it into another table.

The `INSERT INTO SELECT` statement requires that the data types in source and target tables match.

**Note:** The existing records in the target table are unaffected.

### INSERT INTO SELECT Syntax

Copy all columns from one table to another table:

INSERT INTO _table2_  
SELECT * FROM _table1  
_WHERE _condition_;

Copy only some columns from one table into another table:

INSERT INTO _table2_ (_column1_, _column2_, _column3_, ...)  
SELECT _column1_, _column2_, _column3_, ...  
FROM _table1_  
WHERE _condition_;


### LINKS

[[DML (Data Manipulation Language)]]