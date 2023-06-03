# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import pandas library to read csv or excel file.
2. Import LabelEncoder using sklearn.preprocessing library.
3. Transform the data's using LabelEncoder.
4. Import decision tree classifier from sklearn.tree library to predict the values.
5. Find accuracy.
6. Predict the values.
7. End of the program


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: kathirvel.A
RegisterNumber:  212221230047
import pandas as pd
data=pd.read_csv("Employee.csv")

data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:



Initial data set:




![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/b10d1575-3775-4533-b36c-8cbb84149aca)




Data info:

![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/334715f2-5257-464f-b891-d1fec5130a1b)




Optimization of null values:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/78a999ed-d7b7-4fca-9dda-6d1850c44fbc)




Assignment of x and y values:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/8ac7f8e0-ed6b-4d7b-ad4d-cdb9f3b5b99d)



![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/42f344a5-5a74-44e7-8b71-3bf1cfea6c67)




Converting string literals to numerical values using label encoder:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/5ca5f9c6-358a-42ad-92cb-e1828dfd8a84)




Accuracy:



![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/8fbe82b6-3b12-4a03-829f-4dcdd8e9ff01)




Prediction:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/1d1691ed-d0c4-4205-88b3-3610956b79ed)








## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
