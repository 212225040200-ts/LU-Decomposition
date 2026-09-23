# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required library (numpy).
2. Initialize the matrix for which the LU decomposition needs to be found.
3. Apply LU Decomposition
4. Display the results

## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: LINGARAJ B
RegisterNumber: 212225040200
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
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
Developed by: LINGARAJ B
RegisterNumber: 212225040200
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1" 
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
<img width="1019" height="553" alt="image" src="https://github.com/user-attachments/assets/93bea064-f198-45b8-8d31-57e4eb9431f0" />
<img width="880" height="340" alt="image" src="https://github.com/user-attachments/assets/c4534621-92ec-4b30-85f3-3ade2afabc0e" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
