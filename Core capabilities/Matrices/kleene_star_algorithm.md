# kleene_star_algorithm(A : numpy.ndarray, column : int)
An implementation of Kleene star algorithm for calculating the eigenvectors of a matrix.

## Parameters
- `A : numpy.ndarray`: a square NumPy array.
- `column : int`: the column to be used as the eigenvector; defaults to `0`.

## Returns
- `result : numpy.ndarray`: an eigenvector of the matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(kleene_star_algorithm(A))  # -> [[0], [3], [6]]
```
