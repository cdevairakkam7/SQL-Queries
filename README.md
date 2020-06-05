# SQL Queries
This repo contains my SQL queries that will work on [Snowflake](https://www.snowflake.com/) sql engine and other popular sql engines.  
* All sql queries need a table to run against. Here is the [code](https://github.com/cdevairakkam7/SQL_Queries/blob/master/create%20table.md) to create and insert data into the table.

* SQL is a very powerful aggregator. 
  + It can easily sum up numbers.
  + Find minimum & maxium given a set of rows.
  + Do a cumulative addition or subtraction over time
  + The code for the concepts mentioned above can be found [here](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Aggregate%20Functions.md)

* Roles and permissions play a vital part in giving and restricting access to users. [Here](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Granting%20and%20revoking%20access.md) are some examples on granting and revoking access to users.

* There is a keyword called ```CASE``` which can be used as 
  + IF ELSE within a row
  + Transaform content of a cell on the fly 
  + change the datatype of a column and many more.
  + CASE statements can be found [here](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Case%20Statement.md)
  
  * String manupilation is part and parcel of any business setting.
    + strings can be concatenated
    + smaller portion of string can be selected
    + Length of a string can be found
    +Some examples can be found [here](https://github.com/cdevairakkam7/SQL_Queries/blob/master/String%20Manupilation.md)
   
  * Most systems operate in UTC timzone but the business may not be on UTC timezone. With SQL changing timzone is easy.
    + From one timstamp year, month, date, day of week and much more can be extracted.
    + Sample code can be found [here](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Date%20functions.md)
  
  * JOINS connects multiple tables
    + [code](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Joins.md)
   
  * Sometimes complex problems need more than one query. A concepted call nested query can get the job done.
    +[code](https://github.com/cdevairakkam7/SQL_Queries/blob/master/Nested%20Query.md)
