# power(*args : float)
An implementation of the exponentation operation in tropical algebra.
it is equivalent to the `prod` function from the `math` module except for the argument validity check.

## Parameters
- `*args : float`: numerical arguments within the domain.

## Returns
- `result : float`: the product.

# Examples
```Python
from mplusa import minplus as mpa
import math

print(mpa.power(1, 15, 3))  # -> 45
print(mpa.power(3, math.inf))  # -> math.inf
try:
    print(mpa.power(-16, -math.inf))
except:
    print("This would cause an exception.")
```
