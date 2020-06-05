## Inner Join

```
SELECT S1.Unique_ID as Unique_ID,
       Git_TEST.Description as Description,
       Git_TEST.stock,
       Git_TEST.amount
       Git_TEST.Region,
       S1.time_stamp
FROM   Git_TEST INNER JOIN S1
       ON S1.Serial_No = GIT_TEST.Serial_NO
WHERE  S1.time_stamp > 10000000000;
```
