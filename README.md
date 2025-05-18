# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SURYANARAYANAN T
RegisterNumber: 212224040341
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
print(data.head())
x=data[["Position","Level"]]
print(x.head())
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
r2=metrics.r2_score(y_test,y_pred)
print(r2)
dt.predict([[5,6]])
*/
```

## Output:
![image](https://github.com/user-attachments/assets/aad5aca2-1ba3-40d4-8265-ad1577227788)
![image](https://github.com/user-attachments/assets/36cad1ff-52b6-4f54-a3e5-5aa26f872b2f)
![image](https://github.com/user-attachments/assets/836e3b52-b9f2-4516-89e9-5fc1a8237b0f)
![image](https://github.com/user-attachments/assets/fc5b766d-ad86-4a9e-a197-431999496109)
![image](https://github.com/user-attachments/assets/60063972-1051-4836-b97b-1b820b8a0a7b)
![Screenshot 2025-05-18 230109](https://github.com/user-attachments/assets/5e96347b-a35c-44ec-b1c3-c80961d20193)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
