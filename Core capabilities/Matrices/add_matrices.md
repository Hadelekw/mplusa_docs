# add_matrices(A : numpy.ndarray, B : numpy.ndarray)
An implementation of parallel composition (sum) of matrices of the same size.

$$ \left(\mathbf{A} \oplus \mathbf{B}\right)\_{ij} := \mathbf{A}\_{ij} \oplus \mathbf{B}\_{ij} $$

It is equivalent to the `numpy.minimum` or `numpy.maximum` function except for the argument validity check.

## Parameters
- `A : numpy.ndarray`: a 1-dimensional or 2-dimensional NumPy array.
- `B : numpy.ndarray`: a NumPy array of the same shape as `A`.

## Returns
- `result : numpy.ndarray`: a NumPy array with minimal entries.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])
B = np.array([
    [9, 8, 7],
    [6, 5, 4],
    [3, 2, 1],
])

print(mpa.add_matrices(A, B))  # -> [[1, 2, 3], [4, 5, 4], [3, 2, 1]]
```
