## Nested Query
```
SELECT ROUND(((start.start_video_count/total.new_user_count)*100),2) as Percentage
FROM
 (
     SELECT COUNT (event) as start_video_count,
     TO_CHAR(ts,'MonthYYYY') as Month_Year
     FROM events
     WHERE event = 'start_video'
     AND userid
     IN (SELECT OG2.userid
     FROM
 (
     SELECT OG1.userid as userid,
    FROM
 (
       SELECT u.userid as userid,
       TO_CHAR(e.ts,'FMMonthYYYY') as time_stamp,
       RANK () OVER(PARTITION BY u.userid ORDER BY e.ts ASC) as RANK
      FROM users u FULL OUTER JOIN events e ON u.userid = e.userid
 )
       OG1 WHERE OG1.RANK =1
      AND OG1.time_stamp = 'January2017'
 )
OG2
)
) start,
(
SELECT COUNT (event) as new_user_count,
 TO_CHAR(ts,'MonthYYYY') as Month_Year
FROM events
WHERE userid
     IN (SELECT D2.userid
    FROM
 (
     SELECT D1.userid as userid,
     FROM
 (
     SELECT u.userid as userid,
     TO_CHAR(e.ts,'FMMonthYYYY') as time_stamp,
     RANK () OVER(PARTITION BY u.userid ORDER BY e.ts ASC) as RANK
     FROM users u FULL OUTER JOIN events e ON u.userid = e.userid

 )
 D1 WHERE D1.RANK =1
 AND D1.time_stamp = 'January2017'
 )
D2
)
) total 
```
