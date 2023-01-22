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
![WhatsApp Image 2023-01-22 at 17 18 03](https://user-images.githubusercontent.com/119395610/213914209-72dc41f0-ea39-4bf9-b59f-c5aa7f178397.jpg)
![WhatsApp Image 2023-01-22 at 17 18 17](https://user-images.githubusercontent.com/119395610/213914214-19001dc0-e7d1-42eb-beff-31629f3210cd.jpg)
![WhatsApp Image 2023-01-22 at 17 18 28](https://user-images.githubusercontent.com/119395610/213914229-251263c4-6745-40cf-b105-35edaed8b7b8.jpg)





## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

