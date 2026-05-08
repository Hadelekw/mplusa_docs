# tdet(A : numpy.ndarray)
Calculates the tropical determinant of a matrix.

## Parameters
- `A : numpy.ndarray`: the matrix to calculate the determinant for.

## Returns
- `result : float`: the tropical detemrinant of the matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.tdet(A))  # -> 15
```
