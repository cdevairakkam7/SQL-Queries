## Converting Timezones
```
SELECT CASE WHEN Country_code  IN ('JP') THEN CONVERT_TZ(time_stamp,'Japan/Tokyo','US/Pacific')
            WHEN Country_code  IN ('AUS') THEN CONVERT_TZ(time_stamp,'Brisbane/Australia','US/Pacific')
            WHEN Country_code  IN ('DE') THEN CONVERT_TZ(time_stamp,'Munich/Germany','US/Pacific')
            WHEN Country_code  IN ('GBR') THEN CONVERT_TZ(time_stamp,'London/England','US/Pacific')
            WHEN Country_code  IN ('MX') THEN CONVERT_TZ(time_stamp,'Lzcalli/Mexico','US/Pacific')
            WHEN Country_code  IN ('BR') THEN CONVERT_TZ(time_stamp,'Sao Paulo/Brazil','US/Pacific')
            END as Time_stamp
FROM   GIT_TEST;
```

## Millisecond Manipulations
```
SELECT MONTHNAME(time_stamp),
       DAYOFMONTH(time_stamp),
       DAYNAME(time_stamp),
       MONTH(time_stamp),
       YEAR(time_stamp),
       STRFTIME_USEC(time_stamp),
       FORMAT_TIME_USEC(time_stamp),
       MONTHNAME(time_stamp),
       STRFTIME_USEC(time_stamp,'%x') as Date_Representation ,
       STRFTIME_USEC(time_stamp,'%X') as Time_Representation ,
       STRFTIME_USEC(time_stamp,'%a') as Weekday,
       STRFTIME_USEC(time_stamp,'%c') as Date_Time,
       STRFTIME_USEC(time_stamp,'%j') as Day_of_Year,
       STRFTIME_USEC(time_stamp,'%p') as AM_PM

FROM   GIT_TEST;
```

## Date Filtering 
```
Select date_of_entry,
       date_of_entry +10,
       date_of_entry - 10,
       Country_code,
       Venue
FROM   GIT_TEST
WHERE  date_of_entry > '01-MAY-2016';
```
