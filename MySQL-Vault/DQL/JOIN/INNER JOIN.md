## NNER JOIN

The `INNER JOIN` keyword selects records that have matching values in both tables.

## Syntax

SELECT _column_name(s)_   
FROM _table1_   
INNER JOIN _table2   _ON _table1.column_name_ = _table2.column_name_;`

Let's look at a selection of the [**Products**](https://www.w3schools.com/sql/trysql.asp?filename=trysql_products) table:

|ProductID|ProductName|CategoryID|Price|
|---|---|---|---|
|1|Chais|1|18|
|2|Chang|1|19|
|3|Aniseed Syrup|2|10|

And a selection of the [**Categories**](https://www.w3schools.com/sql/trysql.asp?filename=trysql_categories) table:

| CategoryID | CategoryName | Description                                                |
| ---------- | ------------ | ---------------------------------------------------------- |
| 1          | Beverages    | Soft drinks, coffees, teas, beers, and ales                |
| 2          | Condiments   | Sweet and savory sauces, relishes, spreads, and seasonings |
| 3          | Confections  | Desserts, candies, and sweet breads                        |
|            |              |                                                            |

We will join the Products table with the Categories table, by using the `CategoryID` field from both tables:

### Example

Join Products and Categories with the INNER JOIN keyword:

SELECT ProductID, ProductName, CategoryName  
FROM Products  
INNER JOIN Categories ON Products.CategoryID = Categories.CategoryID;

![[2PHOTO.png]]