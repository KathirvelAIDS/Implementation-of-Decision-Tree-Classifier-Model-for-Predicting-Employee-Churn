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
import matplotlib.pyplot as plt
data = pd.read_csv("/content/Dataset-20230524.zip")
data

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss = []

for i in range(1,11):
    kmeans = KMeans(n_clusters = i,init = "k-means++")
    kmeans.fit(data.iloc[:,3:])
    wcss.append(kmeans.inertia_)

plt.plot(range(1,11),wcss)
plt.xlabel("No. of Clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")

km = KMeans(n_clusters = 5)
km.fit(data.iloc[:,3:])

y_pred = km.predict(data.iloc[:,3:])
y_pred

data["cluster"] = y_pred
df0 = data[data["cluster"]==0]
df1 = data[data["cluster"]==1]
df2 = data[data["cluster"]==2]
df3 = data[data["cluster"]==3]
df4 = data[data["cluster"]==4]
plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="yellow",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="pink",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="purple",label="cluster4")
plt.legend()
plt.title("Customer Segments")
*/
*/
```

## Output:
data.head():

![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/73a42024-1c84-4e80-919e-af981f9640f6)

  
  
data.info():

![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/880e8e02-e2ce-4a81-a9d0-7bd4e948cbb1)


NULL VALUES:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/95b60e63-75d7-4f46-a698-ff1c2554eee1)




ELBOW GRAPH:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/06e78297-a1af-412e-8ee0-b269228d9692)





CLUSTER FORMATION:
![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/580c6fe2-1e3e-4055-9f8d-3ff905c3146b)




PREDICICTED VALUE:


![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/9dc71537-8b49-42ca-a34f-4bb0d55c4be7)




FINAL GRAPH(D/O):

![image](https://github.com/KathirvelAIDS/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/94911373/a758ab2e-af9d-4e48-ae2c-c4afbb818f14)










## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
