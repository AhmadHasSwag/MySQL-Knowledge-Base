## The SQL SELECT LIMIT Clause

The limit clause is used to specify the number of records to return.

## Syntax

SELECT select_list
FROM table_name
WHERE ...
ORDER BY ... 
LIMIT number_records 

### Example

Select the first 3 records of the Customers table:

SELECT * FROM Customers  
LIMIT 3;


==important 
if we want start with line three and take only one record after the the line three we should write like that 
select * 
from table name 
limit 3 , 1 ==