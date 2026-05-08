# eigenvalue(A : numpy.ndarray, func : Callable)
Calculates the eigenvalue of a matrix using a given method.

## Parameters
- `A : numpy.ndarray`: a NumPy array representing the matrix.
- `func : Callable`: one of the functions for calculating the eigenvalue. The supported ones are: `power_algorithm` and `karp_algorithm`. It defaults to the first one.

## Returns
- `result : float`: the eigenvalue of the matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.eigenvalue(A, func=mpa.power_algorithm))  # -> 1
print(mpa.eigenvalue(A, func=mpa.karp_algorithm))  # -> 1
```
