### Query to find Average, Minimum, Maximum, Sum and Count of stock.

```{sql}
SELECT AVG(stock) as Average,
       MIN(stock) as Minium_Stock,
       MAX(stock) as MAximum_Stock,
       ROUND(AVG(stock),-1) as Rounded_Average,
       SUM(stock) as Sum,
       COUNT(stock) as Count
FROM git_test;
```

###  Query to find Average, Minimum, Maximum, Sum and Count of stock where sum of stock is greater than 100.

```{sql}
SELECT AVG(amount) as Average,
       MIN(amount) as Minium_Stock,
       MAX(amount) as MAximum_Stock,
       ROUND(AVG(amount),-1) as Rounded_Average,
       SUM(amount) as Sum,
       COUNT(amount) as Count
FROM git_test
       HAVING SUM(stock)>100;
```       

### Cumulatively adding amount after separating by region and ordering the table ascending. 

```{sql}
SELECT SUM(AMOUNT) OVER (PARTITION BY region order by Date_of_Entry ASC ) as Cummulative_Sum,
       Region
FROM   GIT_TEST;
```
