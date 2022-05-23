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
*/
```

## Output:
data.head():


![image](https://user-images.githubusercontent.com/94911373/169771837-8d2c15ff-5f4e-4a33-9dfb-5addf59f7cbc.png)
  
  
  
  
data.info():

![image](https://user-images.githubusercontent.com/94911373/169772180-bd8c80be-9e49-4e4b-9d48-f82a7632878c.png)


data.head() using label encoder:

![image](https://user-images.githubusercontent.com/94911373/169772700-ad207c32-e9f2-4452-abb7-bb6d9885db14.png)




x.head():


![image](https://user-images.githubusercontent.com/94911373/169773637-afc16ead-72e6-4cc3-97e2-a8dc6c1908da.png)

 
 
 
 accuracy
 
 ![image](https://user-images.githubusercontent.com/94911373/169773429-ae51da19-4e63-4dda-8567-df98d08fccd2.png)

 
 
 
 
 



PREDICTION


 ![image](https://user-images.githubusercontent.com/94911373/169773504-2514316f-7f2a-4f58-9e8f-207a21290134.png)









## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
