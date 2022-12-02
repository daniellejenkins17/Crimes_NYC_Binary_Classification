Binary Classification Analysis of NYC Crimes from 2006-2019

Objective:  To use previous NYC crime data to make accurate predictions about whether crimes were attempted or completed...?

Stakeholder: City of New York 
-Will determine where to invest in resources to help reduce crime in these areas, based whether crimes were attempted or completed 

Dataset: NYPD Open Data Crime Complaints from 2006-2019

Features in the Dataset: 
Complaint Date and Time
Crime and Crime Description
Suspect and Victim Demographics 
Police Precinct Location and Location of the Crimes
Borough Where Crime Occurred and Police Station Borough

We created new columns for details of the month, year, and duration of the crime, day of the week

Target: We wanted to look at attempted vs completed crimes and see which features were the most accurate predictors of whether the crime was attempted or completed

-From ___ coefficient, we wanted to.... know which regions were likely to have completed crimes, so that more resources could be allocated to these areas in NYC

Models: 
Logistic Regression
Random Forest with random Oversampler 
Random Forest with SMOTE, with GridSearch feature

XGBoost with SMOTE...? not working 

(pics of confusion matrices and classification reports for each model) 

Conclusion: 

-It is very difficult to predict attempted crimes, and more easy to predict completed crimes based on this dataset 

