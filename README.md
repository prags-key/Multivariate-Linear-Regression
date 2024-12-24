# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
1.Import necessary modules, pandas for data manipulation and linear_model from sklearn for performing linear regression.
2.Use pandas.read_csv() to load the CSV file containing the dataset into a DataFrame
3.Define the independent variables (x) as the columns "Volume" and "Weight"
4.Define the dependent variable (y) as the "CO2" column
5.Create a linear regression object and fit the model using the x and y data.Print the coefficients and intercept of the trained model.
6.Use the trained model to predict the CO2 emission for a given input (e.g., Volume=3300, Weight=1300).Print the predicted value.
```


## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficient",regression.coef_)
print("Intercept",regression.intercept_)
predict=regression.predict([[3300,1300]])
print("CO2 required is",predict)
Registration no:24006285
Name:PRAGATHI KUMAR
```
## Output:

![alt text](<Screenshot 2024-12-23 144532.png>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.