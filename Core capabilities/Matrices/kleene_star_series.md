# kleene_star_series(A : numpy.ndarray, iterations : int)
Calculates all the matrices necessary to calculate the Kleene star value.

## Parameters
- `A : numpy.ndarray`: a square NumPy array.
- `iterations : int`:  an arbitrary amount of iterations to calculate the star for.

## Returns
- `result : list`: list of NumPy arrays generated during the calculations.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

series = mpa.kleene_star_series(A)
for matrix in series:
    print(matrix)
print(mpa.kleene_star(A))  # -> [[0, 2, 3], [4, 0, 6], [7, 8, 0]]
print(mpa.add_matrices(*series))  # -> [[0, 2, 3], [4, 0, 6], [7, 8, 0]]
```
