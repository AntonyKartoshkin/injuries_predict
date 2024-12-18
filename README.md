﻿# injuries_predict
The model predicts the probability of an employee being injured at work in the first year of his/her employment.
The training data was collected using Google forms sent to enterprises through the technosphere safety departments.

All data is anonymized. The composition of features was selected by an expert in the field of labor protection.

FEATURES SET

CAT FEATURES:\
'sex' - Binary: male or female\
'marriage' - Binary feature: Married or Not\
'education' - Education \
'future_education' - Desire to study further\
'revenue' - Income\
'test_period' - Probation period\
'shift' - Shift\
'time_between_jobs' - Break time between first and last job\ 
'count_days_of_holiday' - Number of vacation days per year\
'count_penatlties' - Number of fines for safety violations over the past month (for new employees the value is set to zero)\
'class_condition' - Class of working conditions\
'industrial_workshoop' - Тame of the workshop\
'position' - Postition\

 NUM FEATURES:\
'age' - Age\
'height' - Height\
'weight' - Weight\
'common_experience' - General work experience\
'proff_experience' - Professional work experience\
'interest_score' - Degree of interest in work from 1 to 10\
'useful_score' - The level of "usefulness" of safety briefings according to the employee opinion (from 1 to 10)\
'job_score' - Level of interest in work (from 1 to 10)

The data was pre-processed: categorical features were converted to strings, numeric features were floated, and empty values ​​were removed.\
A gradient boosting model catboost was run on the obtained data.

 FEATURE IMPORTANCE:\
![FETURE IMPORTANCE](https://github.com/user-attachments/assets/718314f1-a9c9-4720-b45c-fdc6ec92ca37)

METRICS ROC AUC:\
![image](https://github.com/user-attachments/assets/c1491be9-b810-4cf3-9fdf-979c0c833a92)


