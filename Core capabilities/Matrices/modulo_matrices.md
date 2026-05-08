# modulo_matrices(A : numpy.ndarray, b : numpy.ndarray)
An implementation of the modulo operation for matrices according to (Obuchowicz, D'Souza, Banaszak, 1998). 
If A is an MxN matrix with non-negative entries and b is an m-element vector with non-negative entries, then B is an MxN matrix defined by:

$$ \mathbf{B}\_{ij} := \mathbf{A}\_{ij} \diamond \mathbf{b}\_{i} $$

## Parameters
- `A : numpy.ndarray`: a NumPy array.
- `b : numpy.ndarray`: a vertical NumPy array of size Mx1.

## Returns
- `result : numpy.ndarray`: a NumPy array of remainders.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
])

print(mpa.modulo_matrices(A, np.array([[1, 2, 3]]).T))  # -> [[0, 0, 0], [0, 1, 0], [1, 2, 0]]
```
