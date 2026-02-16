The `INSERT INTO` statement is used to insert new records in a table.

###  Syntax

1. Specify both the column names and the values to be inserted:

==**INSERT INTO**== _table_name_ (_column1_, _column2_, _column3_, ...)
==**VALUES**== (_value1_, _value2_, _value3_, ...);`

2. If you are adding values for all the columns of the table, you do not need to specify the column names in the SQL query. However, make sure the order of the values is in the same order as the columns in the table. Here, the `INSERT INTO` syntax would be as follows:

==**INSERT INTO**== _table_name_
==**VALUES**== (_value1_, _value2_, _value3_, ...);


### LINKS

[[DML (Data Manipulation Language)]]