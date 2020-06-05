## Concatenating two strings.

```
SELECT 'The Venue is ' || Venue as Venue
FROM GIT_TEST;
```
### Extracting a subset of a string, Replacing a string and finding the length of a string
```
SELECT SUBSTR(time_stamp,1,10) as Seconds,
       REPLACE(country_code,'CA','Canada') as Country_code,
       LENGTH(time_stamp) as Length
FROM   GIT_TEST
```
