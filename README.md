# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. eqn1
4. Compute the y -intercept of the line by using the formula: eqn2
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
import pandas as pd
  from sklearn import linear_model
  df=pd.read_csv("cars (1).csv")
  a=df[['Weight','Volume']]
  b=df[['CO2']]
  regr=linear_model.LinearRegression()
  regr.fit(a,b)
  print("Coefficient: ",regr.coef_)
  print("Intercept:",regr.intercept_)
  print("Account",regr.predict([[3300,1300]]))





```
## Output:
![image](https://github.com/ARAVIND-23/Multivariate-Linear-Regression/assets/138970182/838210c4-4c1a-4523-a82c-b0884fa157f0)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
