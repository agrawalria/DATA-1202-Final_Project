# DATA-1202-Final_Project

## Assignment details
DATA 1202 - DATA ANALYSIS TOOL ANALYTICS 🔬:

INSTRUCTOR - ANTHONY RIDDING :teacher:

ASSIGNMENT - 5 (DATA ARCHIVE) 🗃️

NAME - RIA AGRAWAL 👩‍🎓

STUDENT ID - 100853663 🧑‍🎨

EMAIL ID - RIA.AGRAWAL@DCMAIL.CA 📧

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
Throughout the project, I have learned how different factors affect sleep patterns and provide me insight into the relationship between sleep duration, sleep quality, gender, occupation, sleep disorders, etc.

### What I’ve learned –

- Aggregation and group by helped to calculate average of calculative variable like average age, average sleep    duration, average sleep quality, and other variables for each unique combination of Gender, Occupation and Sleep disorder which help to analyse data as per group and compare the data between different groups.

- JOIN helped me to join both table on primary and foreign keys and helped me to investigate data as a whole and provide the insight about many other factors like each group fitness level and average daily steps and many other metrics.

- After joining and aggregating the data I can investigate the data in multi-dimensional way, able to analyse if there is any outlier and how different occupation at what age gives it time in physical activity and how it is affecting their health and sleep.

### Challenges Faced –

- I took time in checking all the data is complete and inconsistence like if there is any duplicate, null, blanks, zeroes in the dataset.
 
- After analysing the data very well and after consuming much time I am able to find a outlier for a female Engineer who doesn’t have any sleep order and its physical activity is very low.

- I must be very cautious while deriving any conclusion as there are multi-dimensional relationship data.

### What would I do differently next –

- I will try to visualise data so that I can get to know about the outlier and performance of each occupation and to get more insights from the data.

- I will try to collect more data or will add more data source like best time in a day they fell more relaxed while sleeping or time duration of there holidays which provide more insight about their sleep habits and health.

- I will try to do more validation of data with the help of statistics which provide me more balanced data.

### Insight - 
-	Male Software Engineers whose sleep duration is less than 6.1 and quality of sleep is less than 6.1 have insomnia. The other factor that we can see is the average low physical activity of around 30, high stress level of around 8, and fewer daily steps of around 3000.
-	The occupation which has a low physical activity level and low Daily Steps has more chances of having sleep disorders A software Engineer with 3000 daily steps and 30 physical activity level has Insomnia and a teacher with 3500 daily steps and 40 physical activities has Insomnia and Nurse with 4050 daily steps and 37.50 Physical activity level has Sleep Apnea and Insomnia.
-	Each Occupation with the average age range of 38 to 49 has Sleep Apnea (breathing issue while sleeping) while the Ages 28-53 has Insomnia. However, we can see that people aged 27-56 don’t have any sleep disorders because their physical activity level is high around 40-90. 
-	We can also see one outlier in no sleep disorder data where a female engineer has no sleeping disorder at the age of 52 and their physical activity is very low around 30.
