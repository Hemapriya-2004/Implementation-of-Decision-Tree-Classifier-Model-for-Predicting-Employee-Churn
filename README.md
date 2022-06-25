# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## Step 1:
Import pandas module and import the required data set.

## Step 2:
Find the null values and count them.

## Step 3:
Count number of left values.

## Step 4:
From sklearn import LabelEncoder to convert string values to numerical values.

## Step 5:
From sklearn.model_selection import train_test_split.

## Step 6:
Assign the train dataset and test dataset.

## Step 7:
From sklearn.tree import DecisionTreeClassifier.

## Step 8:
Use criteria as entropy.

## Step 9:
From sklearn import metrics.

## Step 10:
Find the accuracy of our model and predict the require values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: R Hemapriya
RegisterNumber:  212221230036

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
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
![output](https://github.com/Hemapriya-2004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/blob/e7c213d3639bf8e12bbfd806d5e660b65e0b01e0/5a.PNG)
![output](https://github.com/Hemapriya-2004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/blob/417bc0a163b037d50530a24dd5e00a55b2179f69/5b.PNG)
![output](https://github.com/Hemapriya-2004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/blob/48a87bcc9c6128ec1e3e08c5b007484ea9795045/5c.PNG)
![output](https://github.com/Hemapriya-2004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/blob/6a35e1628007ba665374c065935b6547884c908f/5d.PNG)
![output](https://github.com/Hemapriya-2004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/blob/a057ad4cb89d2d19eaacb872c81f5ece0785e30e/5e.PNG)
## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
