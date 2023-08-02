```sql
-------Query to apply transformation(join and aggregation) on the 2 tables-----
select dim.Occupation
,dim.Gender
,dim.`Sleep Disorder`
,avg(dim.Age)
,avg(fact.Physical_Activity_Level)
from dim_sleep_health_lifestyle dim 
join fact_sleep_health_lifestyle fact
on dim.`Person ID` = fact.Person_ID
group by dim.Gender,dim.Occupation,dim.`Sleep Disorder`,dim.`BMI Category`; 
```
