# mult(*args : float)
An implementation of the multiplication operation in tropical algebra.
It is equivalent to the built-in `sum` function except for the argument validity check.

## Parameters
- `*args : float`: numerical arguments within the domain.

## Returns
- `result : float`: the sum.

# Examples
```Python
from mplusa import minplus as mpa
import math

print(mpa.mult(1, 15, -3))  # -> 13
print(mpa.mult(15, math.inf))  # -> math.inf
try:
    print(mpa.mult(-math.inf, 13, 42))
except:
    print("This would cause an exception.")
```
