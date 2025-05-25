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
Here is the **10-line algorithm** for your **Multiple Linear Regression using scikit-learn**:

### **Algorithm: Multiple Linear Regression**

1. **Import** the required libraries: `pandas` for data handling and `sklearn.linear_model` for regression.
2. **Read** the dataset (`car (1).csv`) using `pd.read_csv()`.
3. **Extract** the independent variables `x` (e.g., `Volume`, `Weight`).
4. **Extract** the dependent variable `y` (e.g., `CO2 emissions`).
5. **Create** a linear regression model object.
6. **Train** the model using `.fit(x, y)` with the data.
7. **Get** the learned coefficients using `.coef_`.
8. **Get** the model intercept using `.intercept_`.
9. **Predict** CO2 emissions for a new car with volume = 3300 and weight = 1300.
10. **Print** the predicted CO2 value.


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
