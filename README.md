# Udacity Data Analyst Nanodegree <br>No-Show Appointments Analysis
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


## Data Cleaning

Issues Identified:  
1. Convert ScheduledDay from object to datetime64  
2. Convert AppointmentDay from object to datetime64  
3. Show the full PatientId instead of scientific notation  
4. Change the column name of "Handcap" to "Disabled"  
5. Change the column name of "Hipertension" to "Hypertension"  
6. Change SMS_received to yes or no values  

## Exploratory Data Analysis


## Conclusions


## Limitation  

A limitation of this analysis is the time-period available. Because only three months were included in the dataset, it is not possible to provide an analysis representative of the entire year. Other factors may come into play such as changing seasons and weather, school attendance, or holidays, that would not have been accounted for in this dataset.


