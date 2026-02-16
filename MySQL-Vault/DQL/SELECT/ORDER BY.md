The `ORDER BY` keyword is used to sort the result-set in ascending or descending order.

## Syntax

SELECT _column1_, _column2, ..._  
FROM _table_name_   
==**ORDER BY**== _column1, column2, ..._ ASC|DESC;

IMPORTAN 
you can put expiration in order by like this example 

SELECT winner, subject
  FROM nobel
 WHERE yr=1984
 ORDER BY subject IN ('physics','chemistry'),subject,winner 


