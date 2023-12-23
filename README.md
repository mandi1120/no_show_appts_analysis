# WGU Udacity Data Analyst Nanodegree <br>No-Show Appointments Analysis
### By: Amanda Hanway, 12/9/2023 

## Introduction

Dataset Description:
- The No-Show Appointments dataset includes data related to 100k medical appointments in Brazil.  
- The dataset can be used to examine what factors may influece if a patient does or does not attend their medical appointment.  

Source: https://www.kaggle.com/datasets/joniarroba/noshowappointments  

Columns:  
- PatientId: unique identifier for patient  
- AppointmentID: unique identifier for appointment  
- Gender: patient's gender  
- ScheduledDay: on what day the patient set up their appointment  
- AppointmentDay: on what day the patient will attend their appointment  
- Age: patient's age  
- Neighbourhood: indicates the location of the hospital  
- Scholarship: indicates if patient is enrolled in Brasilian welfare program Bolsa Família  
- Hipertension: indicates if patient has hypertension  
- Diabetes: indicates if patient has diabetes  
- Alcoholism: indicates if patient suffers from alcoholism  
- Handcap: indicates if patient has a disability  
- SMS_received: indicates if patient received a text  
- No-show: ‘No’ if the patient showed up to their appointment, ‘Yes’ if they did not show up  

## Questions for Analysis

- Q1: Do no-show appointments occur more often during certain months than others?  
- Q2: Does the text message reminder influence if the patient attends the appointment?  
- Q3: What percentage of total appointments were no-show appointments?  

## Data Wrangling

The following inforamtion was found upon reviewing the dataset:  
- 14 columns and 110,527 rows are present in the dataset. 
- No null values were identified.  
  
## Data Cleaning

Issues Identified:  
1. Convert ScheduledDay from object to datetime64  
2. Convert AppointmentDay from object to datetime64  
3. Show the full PatientId instead of scientific notation  
4. Change the column name of "Handcap" to "Disabled"  
5. Change the column name of "Hipertension" to "Hypertension"  
6. Change SMS_received to yes or no values  

## Exploratory Data Analysis

- Q1: Do no-show appointments occur more often during certain months than others?  
  - May had the highest percentage of no-shows.  
  - June had the lowest percentage of no-shows.  
![image](https://github.com/mandi1120/no_show_appts_analysis/assets/20828566/4e451731-50da-4653-8df5-49de7c0543fe)

- Q2: Does the text message reminder influence if the patient attends the appointment?   
  - The receipt of a SMS text message did not appear to make a positive impact on the attendance.  
  - The no-show rate for patients who received a text was higher than when patients did not receive a text.  
![image](https://github.com/mandi1120/no_show_appts_analysis/assets/20828566/8992f1de-5b1c-4ecb-9dcc-cb1f0289c86f)

- Q3: What percentage of total appointments were no-show appointments?  
  - 80% of total appointments were attended.    
  - 20% of total appointments were no-showed.    
![image](https://github.com/mandi1120/no_show_appts_analysis/assets/20828566/1fc46be6-ab25-4eaa-b350-e65b6f920d23)

## Conclusions

Analysis:

- Of the 110,527 total appointments in the dataset, 20% were no-shows while the remaining 80% were attended.

- Each of the three months studied reported lower counts of no-shows than attended appointments.
  - May had the highest percentage of no-shows, while June had the least.

| Month | No-show	    | Number	| Percent |
|--     |--           |--       |--       |
| Apr   | No	        | 2,602	  | 80      |
|       | Yes	        | 633	    | 20      |
|       | Total	      | 3,235   | 100     |	
| May   | No	        | 64,037  | 79      |
|       | Yes	        | 16,804  | 21      |
|       | Total	      | 80,841  | 100     | 	
| Jun   | No          |	21,569  | 82      |
|       | Yes	        | 4,882	  | 18      |
|       | Total	      | 26,451  | 100     |

- The receipt of a SMS text message did not appear to make a positive impact on the attendance.
  - The no-show rate for patients who received a text was higher than when patients did not receive a text.

| SMS received	| Attended	| No-show	| Total	  | No-show Rate |
| ------------- | --------- | ------- | -----   | ------------ |
| No            |	62,510	  | 12,535  |	75,045  |	17%          |
| Yes	          | 25,698	  | 9,784   |	35,482  | 28%          |
| Total	        | 88,208  	| 22,319	| 110,527	| 20%          |

## Limitation  

A limitation of this analysis is the time-period available. Because only three months were included in the dataset, it is not possible to provide an analysis representative of the entire year. Other factors may come into play such as changing seasons and weather, school attendance, or holidays, that would not have been accounted for in this dataset.


