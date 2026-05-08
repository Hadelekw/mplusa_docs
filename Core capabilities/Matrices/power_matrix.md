# power_matrix(A : numpy.ndarray, k : int)
An implementation of multiple multiplication operation for matrices. Per definition from (Obuchowicz, D'Souza, Banaszak, 1998):

$$ \exists k_0 \forall k \geq k_0: \mathbf{A}\_{\otimes}^{k + 1} := \mathbf{A}\_{\otimes}^{k} $$ 
$$ \mathbf{A}\_{\otimes}^{k} = \mathbf{A} \otimes \mathbf{A}\_{\otimes}^{k - 1}, \quad \mathbf{A}\_{\otimes}^{0} = \mathbf{E} $$

with E being a tropical unit matrix.

## Parameters
- `A : numpy.ndarray`: a square NumPy array.
- `k : int`: an integer value of the exponent.

## Returns
- `result : numpy.ndarray`: a square NumPy array.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

A = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(mpa.power(A, 3))  # -> [[3, 4, 5], [6, 7, 8], [9, 10, 11]]
```
