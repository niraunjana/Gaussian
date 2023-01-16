# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. First, we want to import numpy,then import sys,assume a variable
2. For gaussian elimination method, we want to make 2nd and 3rd column zero.
3. For that we want to make a range according to our program output.
4. Then print the program with correct form then the output will display.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: NIRAUNJANA GAYATHRI G R
RegisterNumber: 22008369
import numpy as np
import sys
n=int(input())
a=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        a[i][j]=float(input())
for i in range(n):
    if a[i][j]==0.0:
        sys.exit('Divide by zero detected!')
    for j in range(i+1,n):
        ratio = a[j][i]/a[i][i]
        for k in range(n+1):
            a[j][k]=a[j][k]-ratio*a[i][k]
x[n-1]=a[n-1][n]/a[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=x[i]=a[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-a[i][j]*x[j]
    x[i]=x[i]/a[i][i]
for i in range(n):
    print('X%d = %0.2f'%(i,x[i]),end=' ')


*/
```

## Output:
file:///home/sec/Pictures/Screenshots/Screenshot%20from%202023-01-16%2016-29-57.png![image](https://user-images.githubusercontent.com/119395610/212662890-c4aa9514-5114-4d10-a95a-c20c3964efdf.png)
file:///home/sec/Pictures/Screenshots/Screenshot%20from%202023-01-16%2016-30-19.png![image](https://user-images.githubusercontent.com/119395610/212662981-71b21b3c-9c44-4c0d-80d5-3921e96d7549.png)




## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

