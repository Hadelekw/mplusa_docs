# normalize_vector(vector : numpy.ndarray)
Normalizes a given vector by subtracting the minimum or maximum value from all the items.

## Parameters
- `vector : numpy.ndarray`: a horizontal or vertical NumPy array representing a vector.

## Returns
- `result : numpy.ndarray`: a normalized array of the same shape as the input.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

eigenvector = mpa.eigenvector(A, func=mpa.kleene_star_algorithm, normalize=False)
print(eigenvector)
print(mpa.normalize_vector(eigenvector))
```
