# modified_kleene_star_algorithm(A : numpy.ndarray)
An implementation of a modified Kleene star algorithm for calculating the eigenvectors of a matrix.
The modification is the usage of Kleene plus in order to find the critical column of the matrix per (Carnia, et al., 2023).

## Parameters
- `A : numpy.ndarray`: a square NumPy array.

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

print(modified_kleene_star_algorithm(A))  # -> [[0], [3], [6]]
```
