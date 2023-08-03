### Data Transformation
-	I didn’t find any issue in data since there is no blank, null or 0 in fact and dim tables, so I didn’t update or deleted any rows. Only, divided Blood_Pressure column into High_Blood_Pressure and Low_Blood_Pressure in excel which I have shown in the Data Extraction document.
  
-	Created 2 tables `dim_sleep_health_lifestyle` and `fact_sleep_health_lifestyle` and done some transformation like, joining both tables which I have mentioned and aggregating some of the columns which is present in fact and Dim tables with average function and then grouping on columns in dim tables using group by, as shown in below query.

Query -
```sql
select dim.Gender

      ,dim.Occupation
      
      ,dim.`Sleep Disorder`
      
      ,avg(fact.sleep_Duration)
      
      ,avg(fact.Quality_of_Sleep) 
      
      ,avg(dim.Age)
      
      ,avg(fact.Physical_Activity_Level)
      
      ,avg(fact.Stress_Level)
      
      ,avg(fact.Daily_Steps)

from dim_sleep_health_lifestyle dim

join fact_sleep_health_lifestyle fact

on dim.`Person ID` = fact.Person_ID

group by dim.Gender,dim.Occupation,dim.`Sleep Disorder`,dim.`BMI Category`;
```

![image](https://github.com/agrawalria/DATA-1202-Final_Project/assets/70374978/f8fc48cd-8119-44aa-a332-e88891f61350)

### Effect on data after transformation–

-	The data now include average Sleep Duration, Quality of Sleep
, Age, Physical Activity Level, Stress Level and Daily Steps for each group of Gender, Occupation and Sleep Disorder
-	By aggregating and joining the data, we can easily compare an individual's sleep duration and quality with the average values of their specific group.

### INSIGHT–

-	Male Software Engineers whose sleep duration is less than 6.1 and quality of sleep less than 6.1 has insomnia. The other factor which we can see is average low physical activity around 30, high stress level around 8 and less daily steps around 3000.
-	The occupation which has low physical activity level and low Daily Steps has more chances of having sleep disorders like the software Engineer with 3000 daily step and 30 physical activity level has Insomnia, teacher with 3500 daily steps and 40 physical activities has Insomnia and Nurse with 4050 daily step and 37.50 Physical activity level has Sleep Apnea and Insomnia.
-	Each Occupation with the average age range of 38 to 49 has Sleep Apnea (breathing issue while sleeping) while the Age 28-53 has Insomnia. Although we can see that Age 27-56 doesn’t have any sleep disorder because their physical activity level is high around 40-90. 
-	We can also see one outlier in none sleep disorder data where a female engineer has no sleeping disorder with the age of 52 and their physical activity is very low around 30.




