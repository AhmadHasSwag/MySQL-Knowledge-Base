The `LIKE` operator is used in a `WHERE` clause to search for a specified pattern in a column.

There are two wildcards often used in conjunction with the `LIKE` operator:

- The percent sign `%` represents zero, one, or multiple characters
- The underscore sign `_` represents one, single character
## Syntax

SELECT _column1, column2, ..._   
FROM _table_name_   
WHERE _columnN_ ==**LIKE**== _pattern_;`


## The _ Wildcard

The `_` wildcard represents a single character.

It can be any character or number, but each `_` represents one, and only one, character.

## The % Wildcard
----

The `%` wildcard represents any number of characters, even zero characters.
### Example

Return all customers from a city that _contains_ the letter 'L':

SELECT * FROM Customers  
WHERE city LIKE '%L%';

------------------
## Starts With
--------------
To return records that starts with a specific letter or phrase, add the `%` at the end of the letter or phrase.
### Example

Select all customers that starts with the letter "a":

SELECT * FROM Customers  
WHERE CustomerName LIKE 'a%';

---------------
## Ends With
---

To return records that ends with a specific letter or phrase, add the `%` at the beginning of the letter or phrase.

### Example

Return all customers that ends with 'a':

SELECT * FROM Customers  
WHERE CustomerName LIKE '%a';

-------------------
## Contains
------------
To return records that contains a specific letter or phrase, add the `%` both before and after the letter or phrase.

### Example

Return all customers that contains the phrase 'or'

SELECT * FROM Customers  
WHERE CustomerName LIKE '%or%';

-----------
## SQL Wildcard Characters

A wildcard character is used to substitute one or more characters in a string.

Wildcard characters are used with the `[LIKE](https://www.w3schools.com/sql/sql_like.asp)` operator. The `LIKE` operator is used in a `WHERE` clause to search for a specified pattern in a column.
## Wildcard Characters

| Symbol | Description                                                  |
| ------ | ------------------------------------------------------------ |
| %      | Represents zero or more characters                           |
| _      | Represents a single character                                |
| []     | Represents any single character within the brackets *        |
| ^      | Represents any character not in the brackets *               |
| -      | Represents any single character within the specified range * |
| {}     | Represents any escaped character **                          |
## Using the [] Wildcard
--------------

The `[]` wildcard returns a result if _any_ of the characters inside gets a match.

### Example

Return all customers starting with either "b", "s", or "p":

SELECT * FROM Customers  
WHERE CustomerName LIKE '[bsp]%';

------------------------
## Using the - Wildcard
--------------------

The `-` wildcard allows you to specify a range of characters inside the `[]` wildcard.

### Example

Return all customers starting with "a", "b", "c", "d", "e" or "f":

SELECT * FROM Customers  
WHERE CustomerName LIKE '[a-f]%';

-------------------
## Microsoft Access Wildcards

The Microsoft Access Database has some other wildcards:

|Symbol|Description|Example|
|---|---|---|
|*|Represents zero or more characters|bl* finds bl, black, blue, and blob|
|?|Represents a single character|h?t finds hot, hat, and hit|
|[]|Represents any single character within the brackets|h[oa]t finds hot and hat, but not hit|
|!|Represents any character not in the brackets|h[!oa]t finds hit, but not hot and hat|
|-|Represents any single character within the specified range|c[a-b]t finds cat and cbt|
|#|Represents any single numeric character|2#5 finds 205, 215, 225, 235, 245, 255, 265, 275, 285, and 295|
