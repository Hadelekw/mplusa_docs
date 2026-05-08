# kleene_plus_series(A : numpy.ndarray, iterations : int)
Calculates all the matrices necessary to calculate the Kleene plus value.

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

series = mpa.kleene_plus_series(A)
for matrix in series:
    print(matrix)
print(mpa.kleene_plus(A))  # -> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(mpa.add_matrices(*series))  # -> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```
