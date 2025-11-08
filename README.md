# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pndas library
### Step2
Import Linear_model from sklearn.
### Step3
Read the CSV file using pandas library
### Step4
Enter the parameters of the linear function.
### Step5
Print the parameters of the linear function.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:
<img width="1034" height="198" alt="Screenshot 2025-11-08 175348" src="https://github.com/user-attachments/assets/72f17e8b-c13f-434f-968f-2df9e8e05446" />
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
