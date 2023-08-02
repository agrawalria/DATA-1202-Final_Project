### After applying all the transformation, I have uploaded the data in a separate table/view using below SQL command.

Query –

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

![image](https://github.com/agrawalria/DATA-1202-Final_Project/assets/70374978/55f9795c-83cd-4cdd-8ffa-5f1d896de602)

### Validate Data loaded in View

- select * from sleep_health_lifestyle_data_foranalyses;

![image](https://github.com/agrawalria/DATA-1202-Final_Project/assets/70374978/4c341250-459a-474c-92dc-1678b741b5d7)

### The reasons for loading the data in this way are as follows:

-	Storing clean data can be used for Analysis by many Analysts when they were using similar data for their problem statement.
-	This table can be Reusable, and we don’t need to do the transformation again and again for the analysis.
-	By separating the data in table ensure that only the cleaned, quality checked data is loaded which reduces the risk of using error and incomplete data.
-	We can retrieve the data and access the data fast because we don’t need to join or do any type of aggregation or create common table expression again, a simple select query retrieve the data fast, compared to using big query and functions.




