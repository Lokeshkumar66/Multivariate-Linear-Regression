# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

Import the required libraries such as pandas and sklearn.

### Step2

Create/load the dataset and separate the independent variables (X) and the dependent/output variable (Y).

### Step3

Split the dataset into training data and testing data using train_test_split().

### Step4

Create a Linear Regression model, train it using the training data, and obtain the regression coefficients.

### Step5

Give new input values to the trained model and use predict() to predict the output.

## Program:
~~~
import pandas as pd 
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print("Predicted value:",regression.predict([[3300,1300]]))
~~~
## Output:

<img width="1550" height="436" alt="Screenshot 2026-09-05 082307" src="https://github.com/user-attachments/assets/e5ea5b97-db9b-4cf8-bc92-b57424766684" />

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
