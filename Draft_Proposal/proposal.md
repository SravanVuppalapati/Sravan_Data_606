## 1. What is your issue of interest (provide sufficient background information)?
To predict and classify the sentence type of offense depending on the offense,age, offense category.Felony crimes carry the possibility of a prison sentence ranging from a year to life in prison and up to the death penalty.Sentences for felonies can range anywhere from one year to life in prison and, in some states and in the federal system, a sentence can include the death penalty (also called capital punishment). Generally speaking, the more serious the crime is, the longer the sentence can be. But other factors, such as a person's prior criminal history, can affect the length of sentence.
## 2. Why is this issue important to you and/or to others?
Felonies have been a major concern in the US in the recent times.Young population are being involved in crime intentionally or unintentionally.Unlike counties,we see many day-to-day crimes in the headlines in the downtowns of major cities.My objective is to let people know what crime they are doing and what sentence they get depending on their age and crime they have committed.
## 3. What questions do you have in mind and would like to answer?
I would like to know which age groups are more involved in felonies.Also I would like to know which offense is often committed by adults.
## 4. Where do you get the data to analyze and help answer your questions?
https://opendata.dc.gov/datasets/DCGIS::felony-sentences/explore
<br />This dataset has been retreived from 'Open Data DC'.This dataset contains all felony counts sentenced from 2010 to 2020 and includes offender demographic information such as gender, race, and age, as well as sentencing information such as the offense, offense severity group, and the type and length of sentence imposed. The dataset is updated annually.
### Features
<br />OBJECTID:( type: esriFieldTypeOID, alias: OBJECTID )
<br />Internal feature number.
<br />RID:( type: esriFieldTypeString, alias: RID, length: 255)
Row number, sequential
<br />GENERIC_CASE_ID: ( type: esriFieldTypeString, alias: GENERIC_CASE_ID, length: 255)
Randomly generated unique identifier for cases
<br />GENERIC_OFFENDER_ID:( type: esriFieldTypeString, alias: GENERIC_OFFENDER_ID, length: 255)
Randomly generated unique identifier for offenders
<br />CHARGE_NUMBER:(type: esriFieldTypeDouble, alias: CHARGE_NUMBER)
Specific charge number within a case
<br />SENTENCE_YEAR (type: esriFieldTypeDouble, alias: SENTENCE_YEAR)
The year the case was sentenced
<br />RACE:(type: esriFieldTypeString, alias: RACE, length: 255)
Race of the accused
<br />GENDER: (type: esriFieldTypeString, alias: GENDER, length: 255)
Gender of accused
<br />AGE_GROUP: (type: esriFieldTypeString, alias: AGE_GROUP, length: 255)
Age group at the time of offense
<br />OFFENSE: (type: esriFieldTypeString, alias: OFFENSE, length: 255)
The offense of conviction within a case
<br />OFFENSE_TYPE: (type: esriFieldTypeString, alias: OFFENSE_TYPE, length: 255)
The category for the offense of conviction
<br />HOMICIDE_TYPE:(type: esriFieldTypeString, alias: HOMICIDE_TYPE, length: 255)
The type of homicide, if the offense was homicide
<br />OFFENSE_SEVERITY_GROUP:( type: esriFieldTypeString, alias:OFFENSE_SEVERITY_GROUP, length: 255)
The sentencing guidelines ranking for the offense of conviction
<br />SENTENCE_TYPE: ( type: esriFieldTypeString, alias: SENTENCE_TYPE, length: 255 )
The type of sentence imposed for the offense of conviction
<br />SENTENCE_IMPOSED_MONTHS: ( type: esriFieldTypeDouble, alias: SENTENCE_IMPOSED_MONTHS)
The prison sentence length imposed in months Not available for indeterminate and life sentences; A value of 1 month may indicate that the defendant may have been sentenced to time served, the actual value of which is not available to the Commission.
<br />SENTENCE_SUSPENDED_MONTHS:(type: esriFieldTypeDouble,alias: SENTENCE_SUSPENDED_MONTHS)
The prison sentence length suspended in months
<br />SENTENCE_TO_SERVE_MONTHS:(type: esriFieldTypeDouble, alias: SENTENCE_TO_SERVE_MONTHS)
The amount of time to serve in prison Not available for indeterminate and life sentences; A value of 1 month may indicate that the defendant may have been sentenced to time served, the actual value of which is not available to the Commission
<br />SENTENCE_PROBATION_MONTHS:(type: esriFieldTypeDouble, alias: SENTENCE_PROBATION_MONTHS )
The probation sentence length imposed in months
<br />VVCA_AMT: ( type: esriFieldTypeDouble, alias: VVCA_AMT )
A court-ordered payment under the Victims of Violent Crime Compensation Act (VVCA) that goes to the Crime Victims Compensation Program
<br />FINE_AMT: ( type: esriFieldTypeDouble, alias: FINE_AMT ) -The amount of court fines imposed
<br />RESTITUTION_AMT: ( type: esriFieldTypeDouble, alias: RESTITUTION_AMT )
The amount of restitution (the amount that the offender is ordered to pay the victim for damages that the victim suffered as a result of the crime)
<br />FINE_SUSPENDED_AMT: ( type: esriFieldTypeDouble, alias: FINE_SUSPENDED_AMT )
The amount of court fines imposed that were suspended
<br />GIS_ID: ( type: esriFieldTypeString, alias: GIS_ID, length: 50 )
<br />GLOBALID: ( type: esriFieldTypeGlobalID, alias: GLOBALID, length: 38 )
<br />CREATOR: ( type: esriFieldTypeString, alias: CREATOR, length: 255 )
<br />CREATED: ( type: esriFieldTypeDate, alias: CREATED, length: 8 )
<br />EDITOR: ( type: esriFieldTypeString, alias: EDITOR, length: 255 )
<br />EDITED: ( type: esriFieldTypeDate, alias: EDITED, length: 8 )
## 5. What will be your unit of analysis?
* Number of felonies by year:
* Felonies count for each offense:
* Felonies count by sentence:
* Felonies by Gender:
* Felonies by count by age:
* Felonies by Number of felonies by felony charge number:
## 6. What kinds of techniques/models do you plan to use (for example, clustering, NLP, ARIMA, etc.)?
* First I would like to clean up data and check for any class imbalances.
* Then I will feature engineer target variables using either One Hot Encoding or Label Encoding whichever is apt to the case.
* Build modelling pipelines for each algorithm I use.
* I intend to use Logistic Regression, Decision Tree Classifier and KNN algorithms.
* Then use grid search for each algorithm to tune hyperparameters and find the best model for each algorithm.
## 7. What outcomes do you intend to achieve (better understanding of problems, tools to help solve problems, predictive analytics with practicle applications, etc)?
I intend to use ROC-AUC curve as a metric to better understand the performance of each model.I am expecting atleast 70% of accuracy for better reliability on this predictions.
