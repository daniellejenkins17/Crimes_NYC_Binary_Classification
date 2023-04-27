# Crimes-NYC

# Binary Classification of NYC Crimes from 2006-2019

# Workflow: 
I made many models, all of which I tried to accurately predict whether a crime would be attempted or completed, based on the features. Of the models that worked well for this dataset, I hyperparameter tuned and tried to optimize on recall. The reason for this was because we wanted to make sure the attempted crimes would be accurately predicted. It was very hard to accurately predict attempted crimes, however, and much easier to predict the completed crimes. This was partly because this dataset was very imbalanced and there were 719,618 completed crimes, compared to 9,550 attempted crimes. I took a sample of this dataset, of 100,000. Then, I made a copy of the cleaned dataset, and increased the sample size to 500,000 and saw how the classification report changed. The results were better overall with the increased sample size, as was expected. 

# Objective:  
To use previous NYC crime data to make accurate predictions about whether crimes were attempted or completed

![Crime Map](https://i.imgur.com/x1JFXzp.png)

# Stakeholder: City of New York 
-Will determine where to invest in resources to help reduce crime in these areas, based whether crimes were attempted or completed 

# Dataset: 
NYPD Open Data Crime Complaints from 2006-2019. After data cleaning, there were 729,168 crimes of which I took samples of 100,000 and 500,000. The sample of 500,000 yielded better results overall.

# Features in the Dataset: 
Complaint Date and Time
Crime and Crime Description
Suspect and Victim Demographics 
Police Precinct Location and Location of the Crimes
Borough Where Crime Occurred and Police Station Borough

We created new columns for details of the month, year, and duration of the crime, day of the week

# Target: 
We wanted to look at attempted vs completed crimes and see which features were the most accurate predictors of whether the crime was attempted or completed

# Exploratory Data Analysis: 

![EDA](https://imgur.com/a/Kv5NH0x)

![Crimes by Borough](https://imgur.com/a/m9hOa9r)

![Attempted vs Completed](https://imgur.com/a/nRNjhJk)

# Crime Map I constructed using Folium: 

![Crime Map](https://i.imgur.com/6NtAYcZ.png)

# More Specific Crime Map I made specifically from NYC Subway Crime Data 

![Subway Crime Map](https://i.imgur.com/r9hLgew.png)

# Models: 
Logistic Regression with GridSearch 
Random Forest with Random Oversampler
Random Forest with Random Undersampler 
Random Forest with SMOTE, with GridSearch 

![Feature Importances](https://imgur.com/ufWxFEq)

# Conclusion: 

-It is very difficult to predict attempted crimes, and more easy to predict completed crimes based on this dataset
-Harassment and robbery are two crimes that are very ambiguous as to whether they were attempted or completed. It is particularly difficult to predict these two crimes 
-A business recommendation is to allocate more resources to the locations with the most completed crimes 

# Model Optimization:
We tried the original sample size of 100,000 for the models. 
Because increasing the models sample size increases the recall score, 
we reran the models with a sample size of 300,000. 
 
# Models that did not work well for this dataset:  
Multinomial Bayes
XGBoost with SMOTE
KNN with GridsearchCV

