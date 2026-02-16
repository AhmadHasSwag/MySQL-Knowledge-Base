
- SQL keywords are NOT case sensitive: `select` is the same as `SELECT`
- # ORDER BY 
	- in order by you can use it in select either was the column in the select or not for example (select name,last name from table name order by id ) so in the example we order the table with id witch is not in the select clause 
	- you can order the table with some functions like len 
- # NULL Value
	- A field with a NULL value is a field with no value.
	- If a field in a table is optional, it is possible to insert a new record or update a record without adding a value to this field. Then, the field will be saved with a NULL value.
	- ### IS NULL Syntax
		SELECT _column_names 
		FROM _table_name_ 
		WHERE _column_name_ ==**IS NULL**==;

	- ### IS NOT NULL Syntax
		SELECT _column_names   
		FROM _table_name_   
		WHERE _column_name_ ==**IS NOT NULL**==;
