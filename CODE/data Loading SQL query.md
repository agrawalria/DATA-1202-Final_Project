```sql
----To create new table/view after transformation-----
Create View Sleep_health_lifestyle_data_ForAnalyses As
select dim.Gender
,dim.Occupation
,dim.`Sleep Disorder`
,avg(fact.sleep_Duration) Avg_Sleep_Duration
,avg(fact.Quality_of_Sleep) Avg_Qulty_sleep
,avg(dim.Age) Avg_Age
,avg(fact.Physical_Activity_Level) Avg_Physcl_Act_lvl
,avg(fact.Stress_Level) Avg_Stress_Lvl
,avg(fact.Daily_Steps) Avg_Dly_Stps
from dim_sleep_health_lifestyle dim 
join fact_sleep_health_lifestyle fact
on dim.`Person ID` = fact.Person_ID
group by dim.Gender, dim.Occupation, dim.`Sleep Disorder`, dim.`BMI Category`;

----------To check data is available in created table/view------
select * from sleep_health_lifestyle_data_foranalyses; --To see the records in View
```
