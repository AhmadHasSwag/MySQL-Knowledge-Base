
## SQL ALTER TABLE Statement

The `ALTER TABLE` statement is used to add, delete, or modify columns in an existing table.

The `ALTER TABLE` statement is also used to add and drop various constraints on an existing table.

---

## ALTER TABLE - ADD Column

To add a column in a table, use the following syntax:

ALTER TABLE _table_name_  
ADD _column_name datatype_;
## ALTER TABLE - DROP COLUMN

To delete a column in a table, use the following syntax (notice that some database systems don't allow deleting a column):

ALTER TABLE _table_name_  
DROP COLUMN _column_name_;

The following SQL deletes the "Email" column from the "Customers" table:

### Example

ALTER TABLE Customers  
DROP COLUMN Email;

---

## ALTER TABLE - RENAME COLUMN

To rename a column in a table, use the following syntax:

ALTER TABLE _table_name_  
RENAME COLUMN _old_name_ to _new_name_;

## ALTER TABLE - ALTER/MODIFY DATA TYPE

To change the data type of a column in a table, use the following syntax:

ALTER TABLE _table_name_  
MODIFY COLUMN _column_name datatype_;

## Change Data Type Example

Now we want to change the data type of the column named "DateOfBirth" in the "Persons" table.

We use the following SQL statement:

ALTER TABLE Persons  
ALTER COLUMN DateOfBirth year;

Notice that the "DateOfBirth" column is now of type year and is going to hold a year in a two- or four-digit format.

---

## DROP COLUMN Example

Next, we want to delete the column named "DateOfBirth" in the "Persons" table.

We use the following SQL statement:
### LINKS
[[DDL (Data Definition Language)]]
