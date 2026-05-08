# eigenvector(A : numpy.ndarray, func : Callable, func_kwargs : dict, normalize : bool)
Calculates the eigenvector of a matrix using a given method.

## Parameters
- `A : numpy.ndarray`: a NumPy array representing the matrix.
- `func : Callable`: one of the functions for calculating the eigenvalue. The supported ones are: `power_algorithm`, `kleene_star_algorithm` and `modified_kleene_star_algorithm`. It defaults to the first one.
- `func_kwargs : dict`: keyword arguments for the used method. Defaults to an empty dictorionary.
- `normalize : bool`: whether or not the returned vector is meant to me normalized. Defaults to `True`.

## Returns
- `result : numpy.ndarray`: the eigenvector of the matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.eigenvector(A, func=mpa.power_algorithm))
print(mpa.eigenvector(A, func=mpa.kleene_star_algorithm))
print(mpa.eigenvector(A, func=mpa.modified_kleene_star_algorithm))
```
