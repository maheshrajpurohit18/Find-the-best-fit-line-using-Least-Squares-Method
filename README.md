# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1. start program

Step 2. Get the independent variable X and dependent variable Y.

Step 3. Calculate the mean of the X -values and the mean of the Y -values.

Step 4. Find the slope m of the line of best fit using the formula. 

<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">

Step 5. Compute the y -intercept of the line by using the formula:

<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">

Step 6. Use the slope m and the y -intercept to form the equation of the line.

Step 7. Obtain the straight line equation Y=mX+b and plot the scatterplot.

Step 8. end program

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: MAHESH RAJ PUROHIT J
RegisterNumber: 212222240058


import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_Mean=np.mean(X)
Y_Mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
  num+=(X[i]-X_Mean)*(Y[i]-Y_Mean)
  denom+=(X[i]-X_Mean)**2
m=num/denom
b=Y_Mean-m*X_Mean
print(m,b)
Y_Pred=m*X+b
print(Y_Pred)
plt.scatter(X,Y)
plt.plot(X,Y_Pred,color="red")
plt.show() 

*/
```

## Output:
![Screenshot 2024-02-17 113228](https://github.com/maheshrajpurohit18/Find-the-best-fit-line-using-Least-Squares-Method/assets/118749665/7813c19d-f3cd-473b-89e2-54d54e56288c)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
