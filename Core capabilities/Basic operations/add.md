# add(*args : float)
An implementation of the addition operation in tropical algebra.
It is equivalent to the built-in `min` function except for the argument validity check.

## Parameters
- `*args : float`: numerical arguments within the domain.

## Returns
- `result : float`: the minimum.

# Examples
```Python
from mplusa import minplus as mpa
import math

print(mpa.add(1, 15, 3, -89))  # -> -89
print(mpa.add(153, math.inf))  # -> 153
try:
    print(mpa.add(-math.inf, 13, 42))
except:
    print("This would cause an exception.")
```
