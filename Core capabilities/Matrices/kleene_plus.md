# kleene_plus(A : numpy.ndarray, iterations : int)
An implementation of Kleene plus operator for tropical algebra.

$$ \mathbf{A}^{+} := \bigoplus\_{k=1}^{\infty} \mathbf{A}\_{\otimes}^{k} $$

## Parameters
- `A : numpy.ndarray`: a square NumPy array.
- `iterations : int`: an arbitrary amount of iterations to calculate the series.

## Returns
- `result : numpy.ndarray`: the resulting NumPy array.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.kleene_plus(A))  # -> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```
