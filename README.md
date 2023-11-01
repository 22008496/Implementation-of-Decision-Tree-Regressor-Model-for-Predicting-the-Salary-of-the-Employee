# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2. Upload the csv file and read the dataset.
3.check for any null values using the isnull() function.
4.  From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: n.magesh
RegisterNumber: 212222040091

import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data[["Salary"]]
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])

*/
```

## Output:
data.head()

![Screenshot 2023-11-01 185549](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/8179c315-c878-46ab-859c-df6d3be8f0dd)

data.info()

![Screenshot 2023-11-01 185559](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/e404b5dc-a9eb-4787-97c0-16edcef16706)

isnull and sum()

![Screenshot 2023-11-01 185608](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/8a0d198c-7ffb-47ff-a316-4dbf373fcd04)

data.info() for salary

![Screenshot 2023-11-01 185619](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/59a5c76d-b160-47b8-a04b-7122a794b7a4)

MSE value

![Screenshot 2023-11-01 185628](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/8cc9743f-dcea-4a06-8857-c8455bf458b4)

R2 value

![Screenshot 2023-11-01 185634](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/d780678f-e964-4ce9-8e44-ab237c3c271c)

prediction value

![Screenshot 2023-11-01 185648](https://github.com/22008496/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119476113/6c7617ab-e896-47d5-b460-5b6ea2a54f50)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
