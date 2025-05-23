# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

## (i) To find the L and U matrix

Step 1: Start the Program

Step 2: numpy for matrix creation and handling.

Step 3: scipy.linalg.lu for LU decomposition.

Step 4: Input the Matrix

Step 5: Take the square matrix A as input.

Step 6: Use eval(input()) to allow entry in Python list format (e.g., [[2,3],[4,5]]).

Step 7: Use lu(A) from SciPy which returns


## (ii) To find the LU Decomposition of a matrix

Step 1: Start the Program

Step 2: numpy for matrix input and handling.

Step 3: lu_factor and lu_solve from scipy.linalg for LU decomposition and solving.

Step 4: Input the coefficient matrix A (square matrix).

Step 5: Input the right-hand side vector or matrix B.

Step 6: Use lu_factor(A) to compute:

        LU: combined LU decomposition matrix,
        
        PV: pivot indices for row permutations.
        
Step 7: Use lu_solve((PV, LU), B) to solve the system Ax = B.

Step 8: Output the result vector x which solves


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

