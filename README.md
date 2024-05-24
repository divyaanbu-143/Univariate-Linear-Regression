# Implementation of Univariate Linear Regression
# Date : 
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. import the NumPy library using the statement import numpy as np.
2. Define the given matrix A
3. Compute the Univariate Linear Regression using np.linalg.inv()
4. print and end the program
## Program
```

   '''
program to find 1-norm of a matrix.
Developed by: A.Divya
Register Number: 2305002007
'''
import numpy as np 
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
Xmean=np.mean(X)
Ymean=np.mean(Y)
num,den=0,0
for i in range (len(X)):
    num +=(X[i]-Xmean)*(Y[i]-Ymean)
    den +=(X[i]-Xmean)**2
m=num/den
c=Ymean-m*Xmean
print(m,c)
Y_pred=m*X+c
print(Y_pred)
plt.scatter(X,Y)
plt.plot(X,Y_pred,color="orange")
plt.show()


```
## Output
![Screenshot 2024-05-24 161113](https://github.com/divyaanbu-143/Univariate-Linear-Regression/assets/155506447/7ed7c742-e355-4ea9-8bf3-8c5206d0020d)
![Screenshot 2024-05-24 161128](https://github.com/divyaanbu-143/Univariate-Linear-Regression/assets/155506447/6b4a4766-cfbf-4e54-9fc2-fdec204b1335)



## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
