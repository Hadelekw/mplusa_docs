# matrix_rank_singular(A : numpy.ndarray)
Calculates the tropical rank of a matrix using a naive method. Per definition from (Develin, Santos, Strumfels, 2005)

## Parameters
- `A : numpy.ndarray`: a square NumPy array representing the matrix.

## Returns
- `result : int`: the tropical rank of the matrix (size of the largest non-singular minor).

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.matrix_rank_singular(A))  # -> 1
```
