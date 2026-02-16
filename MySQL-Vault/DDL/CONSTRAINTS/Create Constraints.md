## SQL Create Constraints

Constraints can be specified when the table is created with the `CREATE TABLE` statement, or after the table is created with the `ALTER TABLE` statement.

### Syntax

CREATE TABLE _table_name_ (  
    _column1 datatype_ _constraint_,  
    _column2 datatype_ _constraint_,  
    _column3 datatype_ _constraint_,  
    ....  
);

---

## SQL Constraints

SQL constraints are used to specify rules for the data in a table.

Constraints are used to limit the type of data that can go into a table. This ensures the accuracy and reliability of the data in the table. If there is any violation between the constraint and the data action, the action is aborted.

Constraints can be column level or table level. Column level constraints apply to a column, and table level constraints apply to the whole table.

The following constraints are commonly used in SQL:

## **SQL Constraints Summary Table**

| Constraint       | Description                                                                       |
| ---------------- | --------------------------------------------------------------------------------- |
| **NOT NULL**     | Ensures that a column cannot contain a NULL value                                 |
| **UNIQUE**       | Ensures all values in a column are different                                      |
| **PRIMARY KEY**  | Combines **NOT NULL** + **UNIQUE** to uniquely identify each row                  |
| **FOREIGN KEY**  | Maintains referential integrity between tables and prevents invalid relationships |
| **CHECK**        | Ensures values in a column satisfy a specific condition                           |
| **DEFAULT**      | Assigns a default value when no value is provided                                 |
| **CREATE INDEX** | Speeds up searching and retrieving data from the database                         |

### LINKS
[[CONSTRAINTS]]