# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

### (i) To find the L and U matrix
## Algorithm

Step 1: Start the Program

Step 2: numpy for matrix creation and handling.

Step 3: scipy.linalg.lu for LU decomposition.

Step 4: Input the Matrix

Step 5: Take the square matrix A as input.

Step 6: Use eval(input()) to allow entry in Python list format (e.g., [[2,3],[4,5]]).

Step 7: Use lu(A) from SciPy

### (ii) To find the LU Decomposition of a matrix

## Algorithm

Step 1: Start the Program

Step 2: numpy for matrix input and handling.

Step 3: lu_factor and lu_solve from scipy.linalg for LU decomposition and solving.

Step 4: Input the coefficient matrix A (square matrix).

Step 5: Input the right-hand side vector or matrix B.

Step 6: Use lu_factor(A) to compute:

LU: combined LU decomposition matrix, PV: pivot indices for row permutations.

Step 7: Use lu_solve((PV, LU), B) to solve the system Ax = B.

Step 8: Output the result vector x which solves Ax = B.

## Program:
```python
'''Program to find L and U matrix using LU decomposition.
Developed by:Karthick . S 
RegisterNumber:212224230114 
'''
import numpy as np
from scipy.linalg import lu
a = np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
```python
'''Program to solve a matrix using LU decomposition.
Developed by:Karthick . S 
RegisterNumber:212224230114 
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)
```


## Output:
![Screenshot 2025-04-22 232318](https://github.com/user-attachments/assets/6a726d10-ea25-4a97-90aa-e92cba46bd70)

![Screenshot 2025-04-22 232422](https://github.com/user-attachments/assets/81e6d9d6-9eb3-45a5-ad59-2a3635519cce)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

