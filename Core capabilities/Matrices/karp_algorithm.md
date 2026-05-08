# karp_algorithm(A : numpy.ndarray)
An implementation of Karp's algorithm for calculating the minimum or maximum cycle mean.

## Parameters
- `A : numpy.ndarray`: a square NumPy array.

## Returns
- `result : float`: the minimum or maximum cycle mean in the matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.karp_algorithm(A))  # -> 1
```
