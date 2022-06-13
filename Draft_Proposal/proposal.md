# Washington DC Felony Sentences
## 1. What is your issue of interest (provide sufficient background information)?
To predict the number of month of sentence and classify the sentence type of offense depending on the offense,age, offense category.Felony crimes carry the possibility of a prison sentence ranging from a year to life in prison and up to the death penalty.Sentences for felonies can range anywhere from one year to life in prison and, in some states and in the federal system, a sentence can include the death penalty (also called capital punishment). Generally speaking, the more serious the crime is, the longer the sentence can be. But other factors, such as a person's prior criminal history, can affect the length of sentence.
## 2. Why is this issue important to you and/or to others?
Felonies have been a major concern in the US in the recent times.Young population are being involved in crime intentionally or unintentionally.Unlike counties,we see many day-to-day crimes in the headlines in the downtowns of major cities.My objective is to let people know what crime they are doing and what sentence they get depending on their age and crime they have committed.
## 3. What questions do you have in mind and would like to answer?
I would like to know which age groups are more involved in felonies.Also I would like to know which offense is often committed by adults.
## 4. Where do you get the data to analyze and help answer your questions?
https://opendata.dc.gov/datasets/DCGIS::felony-sentences/explore
<br />This dataset has been retreived from 'Open Data DC'.This dataset contains all felony counts sentenced from 2010 to 2020 and includes offender demographic information such as gender, race, and age, as well as sentencing information such as the offense, offense severity group, and the type and length of sentence imposed. The dataset is updated annually.
### Features
<br />**OBJECTID**: Internal feature number.
<br />**RID**: Row number, sequential
<br />**GENERIC_CASE_ID**: Randomly generated unique identifier for cases
<br />**GENERIC_OFFENDER_ID**:Randomly generated unique identifier for offenders
<br />**CHARGE_NUMBER**: Specific charge number within a case
<br />**SENTENCE_YEAR**: The year the case was sentenced
<br />**RACE**: Race of the accused
<br />**GENDER**: Gender of accused
<br />**AGE_GROUP**: Age group at the time of offense
<br />**OFFENSE**: The offense of conviction within a case
<br />**OFFENSE_TYPE**: The category for the offense of conviction
<br />**HOMICIDE_TYPE**: The type of homicide, if the offense was homicide
<br />**OFFENSE_SEVERITY_GROUP**:The sentencing guidelines ranking for the offense of conviction
<br />**SENTENCE_TYPE**: The type of sentence imposed for the offense of conviction
<br />**SENTENCE_IMPOSED_MONTHS**: The prison sentence length imposed in months Not available for indeterminate and life sentences; A value of 1 month may indicate that the defendant may have been sentenced to time served, the actual value of which is not available to the Commission.
<br />**SENTENCE_SUSPENDED_MONTHS**: The prison sentence length suspended in months
<br />**SENTENCE_TO_SERVE_MONTHS**: The amount of time to serve in prison Not available for indeterminate and life sentences; A value of 1 month may indicate that the defendant may have been sentenced to time served, the actual value of which is not available to the Commission
<br />**SENTENCE_PROBATION_MONTHS**: The probation sentence length imposed in months
<br />**VVCA_AMT**: A court-ordered payment under the Victims of Violent Crime Compensation Act (VVCA) that goes to the Crime Victims Compensation Program
<br />**FINE_AMT**: The amount of court fines imposed
<br />**RESTITUTION_AMT**: The amount of restitution (the amount that the offender is ordered to pay the victim for damages that the victim suffered as a result of the crime)
<br />**FINE_SUSPENDED_AMT**: The amount of court fines imposed that were suspended
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
