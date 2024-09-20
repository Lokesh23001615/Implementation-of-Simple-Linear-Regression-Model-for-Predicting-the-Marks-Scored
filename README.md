# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1. Start the program.

Step 2. To implement the linear regression using the standard libraries in the python.

Step 3. Use slicing function() for the x,y values.

Step 4. Using sklearn library import training , testing and linear regression modules.

Step 5. Predict the value for the y.

Step 6. Using matplotlib library plot the graphs.

Step 7. Use xlabel for hours and ylabel for scores.

Step 8. End the porgram.
## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Lokesh M
RegisterNumber:  212223230114

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
df=pd.read_csv('/content/student_scores - student_scores.csv')
df.head()
X=df.iloc[:,:-1].values
X
y=df.iloc[:,1].values
y
from sklearn.model_selection import train_test_split
X_train,X_test,y_train,y_test=train_test_split(X,y,test_size=1/3,random_state=0)
from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(X_train,y_train)
y_pred=regressor.predict(X_test)
y_pred
y_test
plt.scatter(X_train,y_train,color='violet')
plt.plot(X_train,regressor.predict(X_train),color="black")
plt.title("h vs s (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(X_test,y_test,color='purple')
plt.plot(X_test,regressor.predict(X_test),color="black")
plt.title("h vs s (Testing Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
*/
```

## Output:
![Screenshot 2024-09-04 143806](https://github.com/user-attachments/assets/ecaaec3f-5c7f-464f-af9e-c192cfc998ca)

![Screenshot 2024-09-04 143814](https://github.com/user-attachments/assets/e71037db-d3e1-4a05-8480-df07a7adb421)


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
