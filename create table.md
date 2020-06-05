# Create Table Sql Query
``` *.sql
create table Git_test
(Serial_no number,
unique_ID varchar2(13),
description varchar2(20),s
tock number,
amount number,
venue varchar2(20),
country_code varchar2(20),
region varchar2(20),
Date_of_Entry date, 
time_stamp number);
```

## I have intentionally created a table with popular data types that are used in everyday business.

# Inserting data into the table

``` {sql}
insert into GIT_TEST values (1,'A1','Initial Stock',1000,1000,'Atlanta','US','NA','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (2,'B2','Purchase',70,175,'London','GBR','EMEA','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (3,'C3','Carry Over',293,845,'Munich','DE','EMEA','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (4,'D4','Damaged',1000,1000,'Brisbane','AUS','APAC','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (5,'E5','Returned',1000,1000,'Tokyo','JP','APAC','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (6,'F6','Initial Stock',1000,1000,'Sao Paulo','BR','LATAM','30-DEC-2016',1483155367000000);
insert into GIT_TEST values (7,'G7','Initial Stock',1000,1000,'Metepec','MX','LATAM','29-DEC-2016',1483068967000000);
insert into GIT_TEST values (8,'H8','Carry Over',1000,1000,'Qubec','CA','NA','30-DEC-2016',1483155367000000);
insert into GIT_TEST values (9,'I9','Initial Stock',1000,1000,'Tampa','US','NA','27-DEC-2016',1482896167000000);
insert into GIT_TEST values (10,'J10','Returned',1000,1000,'Montreal','CA','NA','01-JAN-2017',1483328167000000);
insert into GIT_TEST values (11,'K11','Initial Stock',1000,1000,'Lzcalli','MX','LATAM','15-DEC-2011',1479267367000000);
insert into GIT_TEST values (12,'L12','Purchase',1000,1000,'Salvador','BR','LATAM','11-DEC-2016',1478921767000000);
insert into GIT_TEST values (13,'M13','Initial Stock',1000,1000,'Kyoto','JP','APAC','1-NOV-2016',147805416700000);
insert into GIT_TEST values (14,'N14','Damaged',1000,1000,'Sydney','AUS','APAC','10-DEC-2016',1481427367000000);
insert into GIT_TEST values (15,'O15','Initial Stock',1000,1000,'Frankfurt','DE','EMEA','27-DEC-2016',1482896167000000);
insert into GIT_TEST values (16,'P16','Returned',1000,1000,'New Castle','GBR','EMEA','20-DEC-2016',1482291367000000);
insert into GIT_TEST values (17,'Q17','Carry Over',1000,1000,'Venice','ITA','EMEA','20-DEC-2016',1482291367000000);
insert into GIT_TEST values (18,'R18','Purchase',1000,1000,'Melbourne','AUS','APAC','20-DEC-2016',1482291367000000);
insert into GIT_TEST values (19,'S19','Damaged',1000,1000,'Hiroshima','JP','APAC','20-DEC-2016',1482291367000000);
insert into GIT_TEST values (20,'T20','Carry Over',1000,1000,'Miami','US','NA','20-DEC-2016',1482291367000000);
```
