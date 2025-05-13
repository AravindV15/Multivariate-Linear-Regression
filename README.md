# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import the required libraries: pandas for data manipulation and linear_model from sklearn for regression.

### Step2
<br>Load the dataset using pd.read_csv() and store it in a DataFrame.

### Step3
<br>Separate the features (independent variables) and the target (dependent variable):

Assign the relevant columns to X (features).
Assign the target column to y (output).

### Step4
<br>
Create a linear regression model using linear_model.LinearRegression() and fit it to the data using regr.fit(X, y).
### Step5
<br>Print the regression coefficients (regr.coef_) and intercept (regr.intercept_).
Use the trained model to make predictions using regr.predict() with the given input values.
Display the predicted output.
## Program:
```
# Developed by: Mohana k.v.s.l
# Reg no: 24900659

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

##output:
![Screenshot 2025-05-01 163943](https://github.com/user-attac


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.



