# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Import pandas as pd and import linear_model from sklearn
2. Read the csv file.
3. Get the value of x and y variables.
4. Create the linear regression model and fit.
5. Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm cube.
6. Print the predicted output.

## Program:
```
Developed by:Karthikeyan C
Register no: 212224040152
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
![alt text](<Screenshot 2025-05-22 143617.png>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.