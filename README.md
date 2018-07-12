# census-income-prediction

Adult-Census-Income
Purpose:
This project is to predict a person's salary lies in either 50K+ or 50K-.

1.1 Data Extraction
The Adult-Census-Income is from UCI:
https://archive.ics.uci.edu/ml/machine-learning-databases/adult/

Dataset Features:

age, workclass, fnlwgt, education,	education-num, marital-status, occupation, relationship, race, sex	, capital-gain, capital-loss, hours-per-week	, native-country, class

The class Feature is the label we want to predict which contains salary of a person

1.2 Data Preprocess

*Imputing Missing Values
 we have deleted the missing value which was given as "?" as they were in less percentage

*Convert categorical values into numerical values.
Method: Label Encoding

1.3 Model Selection

Logistic regression with imbalance data
Overall Test Accuracy is 0.79.

*Dealing with Imbalanced Data
Salary Feature is unbalanced labeled. 
The salary > 50k is around 30% and <= 50K is 70%.
Method: SMOTE method 

Logistic regression after applying SMOTE technique 
Overall Test Accuracy is 0.87.
