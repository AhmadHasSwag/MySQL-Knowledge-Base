


## Definition and Usage

The CHAR_LENGTH() function return the length of a string (in characters).

## Syntax

CHAR_LENGTH(_string_)

### Example

Return the length of the string:

SELECT CHAR_LENGTH("SQL Tutorial") AS LengthOfString;


---

### Example

Return the length of the text in the "CustomerName" column:

SELECT CHAR_LENGTH(CustomerName) AS LengthOfName  
FROM Customers;

### LINKS
[[STRING FUNCTIONS]]
