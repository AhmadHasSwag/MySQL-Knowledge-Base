## SQL Comments

Comments are used to explain sections of SQL statements, or to prevent execution of SQL statements.

**Note: Comments are not supported in Microsoft Access databases!**

---

## Single Line Comments

Single line comments start with `--`.

Any text between -- and the end of the line will be ignored (will not be executed).

The following example uses a single-line comment as an explanation:

### Example

-- Select all:  
SELECT * FROM Customers;
## Multi-line Comments

Multi-line comments start with `/*` and end with `*/`.

Any text between /* and */ will be ignored.

The following example uses a multi-line comment as an explanation:

### Example

/*Select all the columns  
of all the records  
in the Customers table:*/  
SELECT * FROM Customers;