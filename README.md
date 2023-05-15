# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import dataset and get data info
2. check for null values
3. Map values for position column
4. Split the dataset into train and test set
5. Import decision tree regressor and fit it for data
6. Calculate MSE,R2 and y predict
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:S.SRIMATHI
RegisterNumber:212220040160  

import pandas as pd

data=pd.read_csv('/content/Salary.csv')

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

y.head()

from sklearn.model_selection import train_test_split

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=200)

from sklearn.tree import DecisionTreeRegressor

dt=DecisionTreeRegressor()

dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics

mse=metrics.mean_squared_error(y_test,y_pred)

mse

r2=metrics.r2_score(y_test,y_pred)

r2

dt.predict([[5,6]])
*/
```

## Output:

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/87b2ba17-52e8-4a53-b438-0d2cf80ccd01)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/0df06e4b-0f98-493d-a6f6-dcfc53c86c5e)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/8b9318cc-6b7b-4711-967e-372aae0d4f9b)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/347f5bc6-63cb-4dc2-a3de-5a1aba5db7d8)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/dabf6354-4c36-435d-ad05-07808d5eb4d7)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/2540fe10-3f30-45c0-8660-21190c101c26)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/6b33022d-7765-4171-9472-b28eaf01985a)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/430d312a-1cd7-409e-b574-c578ea373037)

![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/114581999/d6a3396b-a627-454f-89f1-41f59f76a104)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
