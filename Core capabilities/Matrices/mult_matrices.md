# mult_matrices(A : numpy.ndarray, B : numpy.ndarray)
An implementation of series composition (product) of matrices of sizes `MxN` and `NxP`.

$$ \left(\mathbf{A} \otimes \mathbf{B}\right)\_{ij} := \bigoplus\_{k=1}^{N}\left(\mathbf{A}\_{ik} \otimes \mathbf{B}\_{kj}\right) $$

## Parameters
- `A : numpy.ndarray`: a NumPy array of shape MxN.
- `B : numpy.ndarray`: a NumPy array of shape NxP.

## Returns
- `result : numpy.ndarray`: a NumPy array of shape MxP.

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

print(mpa.mult_matrices(A, B))  # -> [[6, 5, 4], [9, 8, 7], [12, 11, 10]]
```
