# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1:
 Import numpy libary using import statement.
Step 2:
From scipy package import lu().
Step 3:
Get input from user and pass it as an array.
Step 4:
Get P,L U matrix using lu().
Step 5:
End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Pooja.P
RegisterNumber: 212224100041
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Pooja.P
RegisterNumber: 212224100041
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
pv,lu=lu_factor(A)
result=lu_solve((pv,lu),B)
print(result)

```

## Output:
![alt text](<Screenshot 2025-04-16 183704.png>)
![alt text](<Screenshot 2025-04-16 183736.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

