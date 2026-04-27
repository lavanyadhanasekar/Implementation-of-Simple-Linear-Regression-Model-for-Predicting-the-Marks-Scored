# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import required libraries
2.Take input dataset (e.g., study hours vs marks scored)
3.Reshape data for model training
4.Split dataset into training and testing sets
5.Create a Linear Regression model
6.Train the model using training data
7.Predict marks using test data
8.plot the regression line and data points
9.Display predicted results
  
  

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: 
RegisterNumber:  
*/

# Program to implement simple linear regression model
# Developed by:lavanya D
# Register Number:212225040195

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression


X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])


model = LinearRegression()

model.fit(X, Y)


Y_pred = model.predict(X)


print("Slope (m):", model.coef_[0])
print("Intercept (b):", model.intercept_)


plt.scatter(X, Y, color='blue', label='Actual Data')
plt.plot(X, Y_pred, color='red', label='Regression Line')
plt.xlabel("Study Hours")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression - Marks Prediction")
plt.legend()
plt.show()
```

## Output:

<img width="766" height="613" alt="image" src="https://github.com/user-attachments/assets/24c53306-ad48-4649-95fc-7d73a33272da" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
