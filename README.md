# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import required libraries and load the dataset.

### Step2
Define the feature matrix and target vector.

### Step3
Split the dataset into training and testing sets.

### Step4
Create a Linear Regression model and train it using training data.

### Step5
Predict outputs, evaluate the model, and plot the residual errors.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:

<img width="1279" height="447" alt="Screenshot 2026-08-22 233031" src="https://github.com/user-attachments/assets/378b3d81-af39-4205-8c0e-b4f5f0adbf71" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
