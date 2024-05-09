# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import pandas as pd.

### Step2
<br>
Read the csv file.

### Step3
<br>
Get the value of x and y variables.

### Step4
<br>
Create the linear regression model and fit

### Step5
<br>
Predict the CO2 emission of a car where the weight is 3300kg and the volume is 1300cm cube.

## Program:
```
## Developed by S.Hemavathy
## Register No: 212223230076

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount",regr.predict([[3300,1300]]))

```
## Output:
![883bd2eb-e67d-41a7-8a54-b27055c09870](https://github.com/Hemaatchu/Multivariate-Linear-Regression/assets/147328300/32e52225-32cc-4ab0-b9e2-acbf63ebfea7)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
