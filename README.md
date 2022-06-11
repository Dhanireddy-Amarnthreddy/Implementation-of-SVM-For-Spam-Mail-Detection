# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.  Import the required packages.
2. Import the dataset to operate on.
3. Split the dataset.
4. Predict the required output.
5.End the program
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: D.Amarnath Reddy
RegisterNumber: 212221240012


import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:

<img width="632" alt="11" src="https://user-images.githubusercontent.com/94165103/173193263-1002aa12-9a82-43b8-99b4-2d721769aa85.png">


<img width="640" alt="12" src="https://user-images.githubusercontent.com/94165103/173193267-37b836eb-4347-456b-b3c8-7e083eaa1d8a.png">

<img width="326" alt="13" src="https://user-images.githubusercontent.com/94165103/173193274-5424ae58-cf1a-4a4e-86f6-3ac4f0aeb8bd.png">

<img width="633" alt="14" src="https://user-images.githubusercontent.com/94165103/173193293-87d046bb-8753-4ab5-a965-659bb314f064.png">

<img width="338" alt="15" src="https://user-images.githubusercontent.com/94165103/173193295-34f29eed-5645-4873-b1da-e3259e1b675c.png">


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
