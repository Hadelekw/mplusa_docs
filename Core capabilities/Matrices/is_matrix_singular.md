# is_matrix_singular(A : numpy.ndarray)
Performs a naive check of tropical matrix singularity.

## Parameters
- `A : numpy.ndarray`: a square NumPy array representing the matrix.

## Returns
- `result : bool`: whether or not the matrix is singular.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [0, 1],
    [1, 0],
])

print(mpa.is_matrix_singular(A))  # -> False

A = np.array([
    [0, 1],
    [-1, 0],
])

print(mpa.is_matrix_singular(A))  # -> True
```
