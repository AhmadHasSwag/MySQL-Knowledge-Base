## The SQL CREATE TABLE Statement

The `CREATE TABLE` statement is used to create a new table in a database.

### Syntax

CREATE TABLE _table_name_ (  
    _column1 datatype_,  
    _column2 datatype_,  
    _column3 datatype_,  
   ....  
);
## Create Table Using Another Table

A copy of an existing table can also be created using `CREATE TABLE`.

The new table gets the same column definitions. All columns or specific columns can be selected.

If you create a new table using an existing table, the new table will be filled with the existing values from the old table.

### Syntax

CREATE TABLE _new_table_name_ AS  
    SELECT _column1, column2,..._  
    FROM _existing_table_name_  
    WHERE ....;

The following SQL creates a new table called "TestTable" (which is a copy of the "Customers" table): 

### Example

CREATE TABLE TestTable AS  
SELECT customername, contactname  
FROM customers;

### LINKS
[[DDL (Data Definition Language)]]