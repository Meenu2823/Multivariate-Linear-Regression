# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Importing pandas and scikit-learn libraries.

### Step2
<br>Reading the data from a CSV file.

### Step3
<br>Splitting the data into features (X) and target (y).

### Step4
<br>Creating and fitting the linear regression model.

### Step5
<br>Print the coefficients and intercept of the linear regression model.

### Step6
<br>Making a prediction.

### Step7
<br>Printing the predicted CO2 emissions.


## Program:
```python
#Program to implement multivariate linear regression
#Developed by : Meenu.S
#Register nuumber:23003303
import pandas as pd
from sklearn import linear_model

df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercepts:",regr.intercept_)
predictedco2=regr.predict([[3300,1300]])
print("Predicted co2 for the corresponding weight and volume",predictedco2)


```
## Output:

![Alt text](<Maths exp-10.png>)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.