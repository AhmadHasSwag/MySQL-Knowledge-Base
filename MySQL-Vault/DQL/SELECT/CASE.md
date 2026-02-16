## The SQL CASE Expression

The `CASE` expression goes through conditions and returns a value when the first condition is met (like an if-then-else statement). So, once a condition is true, it will stop reading and return the result. If no conditions are true, it returns the value in the `ELSE` clause.

If there is no `ELSE` part and no conditions are true, it returns NULL.

## CASE Syntax

CASE  
    WHEN _condition1_ THEN _result1_  
    WHEN _condition2_ THEN _result2_  
    WHEN _conditionN_ THEN _resultN_  
    ELSE _result_  
END;

### LINKS
[[SELECT]]
