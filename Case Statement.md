## CASE statment is used as a lookup function in the following query.

```
SELECT Country_code,
       CASE  WHEN Venue IN ('Atlanta','Qubec','Tampa','Montreal','Miami') THEN 'North America'
             WHEN Venue IN ('Brisbane','Tokyo','Kyoto','Sydney','Melbourne','Hiroshima') THEN 'Asia Pacific'
             WHEN Venue IN ('Sao Paulo','Metepec','Lzcalli','Salvador') THEN 'Latin America'
             ELSE 'EMEA' END as Business_Region
FROM   GIT_TEST
GROUP BY Country_code,Venue;
```

## CASE statment is used in the WHERE clause  against multiple conditions to get the resultant set

```
SELECT Unique_ID,
       Description,
       Stock,
       Amount,
       Venue,
       Country_code,
       Region,
       Date_of_Entry
FROM   GIT_TEST
WHERE  CASE COUNTRY_CODE WHEN COUNTRY_CODE IN ('CA','US') THEN Amount >999
            WHEN COUNTRY_CODE IN ('AUS','JP') THEN stock >500
            WHEN COUNTRY_CODE IN ('AUS','JP') THEN stock >500
            WHEN COUNTRY_CODE IN ('MX','ITA') THEN Description IN ('Initial Stock','Carry Over')
      END;
```
