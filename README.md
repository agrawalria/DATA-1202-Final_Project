# DATA-1202-Final_Project
## About Project
This is a DATA-1202 Project where we will take 2 datasets through which we analyze the relationship between sleep, health, and lifestyle and how they are affecting each other.

## DATA SOURCE USED
The Dataset is taken from Kaggle and it's in CSV format. 
### Dataset Overview:
The sleep health and lifestyle dataset has 400 rows and 13 columns, covering a wide range of variables related to sleep and daily habits. This includes details such as gender, age, occupation, hours slept, quality of sleep, physical activity, stress level, BMI category, blood pressure, heart rate, steps taken each day, and sleep disturbances.
### Dataset Columns:
- Person ID: An identifier for each individual.
- Gender: The gender of the person (Male/Female).
- Age: The age of the person in years.
- Occupation: The occupation or profession of the person.
- Sleep Duration (hours): The number of hours the person sleeps per day.
- Quality of Sleep (scale: 1-10): A subjective rating of the quality of sleep, ranging from 1 to 10.
- Physical Activity Level (minutes/day): The number of minutes the person engages in physical activity daily.
- Stress Level (scale: 1-10): A subjective rating of the stress level experienced by the person, ranging from 1 to 10.
- BMI Category: The BMI category of the person (e.g., Underweight, Normal, Overweight).
- Blood Pressure (systolic/diastolic): The blood pressure measurement of the person, indicated as systolic pressure over diastolic pressure.
- Heart Rate (bpm): The resting heart rate of the person in beats per minute.
- Daily Steps: The number of steps the person takes per day.
- Sleep Disorder: The presence or absence of a sleep disorder in the person (None, Insomnia, Sleep Apnea-breathing pause while sleeping).
### Key Feature of Dataset:
- Sleep Metric
- Cardiovascular Health
- Lifestyle Factors
- Sleep disorder Analysis

## STEP FOLLOWED
- Extract data from the sources and import it into the database MySQL. 
- Apply some transformation to clean and make the data useful using SQL query.
- Load useful data in the target for further analysis by analysts and create reports to provide insight into the business problems.

## OUTCOMES
Throughout the project, I have learned how different factors affect sleep patterns and provide me insight into the relationship between sleep duration, sleep quality, gender, occupation, sleep disorders, etc. Below are the insights I got from the data that I have used -
-	Male Software Engineers whose sleep duration is less than 6.1 and quality of sleep is less than 6.1 have insomnia. The other factor that we can see is the average low physical activity of around 30, high stress level of around 8, and fewer daily steps of around 3000.
-	The occupation which has a low physical activity level and low Daily Steps has more chances of having sleep disorders A software Engineer with 3000 daily steps and 30 physical activity level has Insomnia and a teacher with 3500 daily steps and 40 physical activities has Insomnia and Nurse with 4050 daily steps and 37.50 Physical activity level has Sleep Apnea and Insomnia.
-	Each Occupation with the average age range of 38 to 49 has Sleep Apnea (breathing issue while sleeping) while the Ages 28-53 has Insomnia. However, we can see that people aged 27-56 don’t have any sleep disorders because their physical activity level is high around 40-90. 
-	We can also see one outlier in no sleep disorder data where a female engineer has no sleeping disorder at the age of 52 and their physical activity is very low around 30.