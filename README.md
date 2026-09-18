# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

Start and import the required libraries such as NumPy, Pandas, and Scikit-learn.

### Step2

Load the dataset and separate the independent variables (X) and dependent variable (Y).

### Step3

Create the Multivariate Linear Regression model using the training data.

### Step4

Train the model using the fit() method and calculate the regression coefficients.

### Step5

Predict the output for new input values using predict() and display the results.

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
