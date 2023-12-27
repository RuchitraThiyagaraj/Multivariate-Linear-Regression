# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Get the independent variable X aand dependent variable Y.
<br>

### Step2
Import pandas as pd and also import linear_model from sklearn module.
<br>

### Step3
Read the CSV file which should be attached to the code runner.
<br>

### Step4
Give the commands to print LinearRegression and also the predicted CO2 for corresponding weights
<br>

### Step5
End the program
<br>

## Program:
```
'''
#Program to implement multivariate linear regression and predict the output.
#Developed by:RUCHITRA THIYAGARAJ
#RegisterNumber:23000100
'''
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars (1).csv")
X=df[['Weight','Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

```
## Output:

### Insert your output
![image](https://github.com/RuchitraThiyagaraj/Multivariate-Linear-Regression/assets/154776996/9fb4c469-7b75-4eec-86ea-997bab530396)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
