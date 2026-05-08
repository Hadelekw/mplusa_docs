# unit_matrix(width : int, height : int)
Generates a two dimensional tropical unit matrix. It is defined as:

$$ \mathbf{E}_{ij} := \begin{cases} 0, &i = j\\ t, &i \neq j \end{cases} $$

where t is the zero unit for a given semiring; infinity for (min, +) and negative infinity for (max, +).

## Parameters
- `width : int`: the width of the unit matrix.
- `height : int`: the height of the unit matrix.

## Returns
- `result : numpy.ndarray`: a NumPy array tropcial unit matrix.

# Examples
```Python
from mplusa import minplus as mpa
import numpy as np

print(mpa.unit_matrix(5, 5))
```
