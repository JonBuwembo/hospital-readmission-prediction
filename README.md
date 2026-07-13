# hospital-readmission-prediction

## Project Status
🚧 In Progress
- [x] Dataset exploration
- [ ] Data cleaning
- [ ] Feature engineering
- [ ] Model development
- [ ] Model evaluation
- [ ] Model deployment

## Project Overview
Hospital readmissions are a major challenge for healthcare systems. Patients who are readmitted shortly after discharge often require additional treatment, increasing healthcare costs and potentially indicating that their initial care or discharge planning was not fully effective. Predicting which patients are at high risk of readmission can help hospitals improve patient outcomes and allocate resources more efficiently.

## Goal
Develop a machine learning classification model that predicts whether a patient will be readmitted to the hospital within 30 days after discharge using demographic, diagnostic, and hospital utilization data.

## What is the dataset?
This dataset contains over **100,000 hospital encounters** for diabetic patients admitted to **130 U.S. hospitals** between 1999 and 2008. Each row represents a single hospital encounter and includes demographic information, diagnoses, medications, laboratory procedures, and hospital utilization data. The objective is to predict whether a patient will be readmitted within 30 days after discharge.

## Who collected it?
The dataset was compiled from electronic health records collected from 130 U.S. hospitals between 1999 and 2008 and later published by researchers in BioMed Research International.

## What healthcare problem does it represent?
Healthcare readmissions are both costly for providers and patients. Predicting readmission risk allows hospitals to identify high-risk patients before discharge so that they can provide additional care, follow-up appointments, or other interventions that may reduce avoidable readmissions and improve patient outcomes.

## What is the prediction target?
The target variable is readmission. 
Possible values:
- <30 if the patient was readmitted within 30 days.
- >30 if the patient was readmitted in more than 30 days
- NO If there are no records of readmission.
  
## How many rows and columns are there?
- 101766 rows
- 50 columns

## Selected Features/Predictors?
- `diabetesMed` (Whether the patient recieved diabetic medication)
- `readmitted` (Target Variable)
- `change` (if there is a change in diabetic medication (values change/no change)
- `number_emergency` (number of emergency visits of the patient preceding the encounter)
- Outpatient visits
- Inpatient visits
- age
- race
- weight
- `time_in_hospital` (amount of days)
- metformin (If the drug was prescribed or there was a change in the dosage) (up, down, steady, no)
  
## What limitations does the data have?
- The data covers the period from 1999–2008 and may not fully represent current clinical practices.
- The data is observational and cannot establish casual relationships
- The dataset only contains diabetic patients, so the model may not generalize well to all hospital populations.

