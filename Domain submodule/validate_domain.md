# validate_domain(value : Any)
Recursive numerical values validation for the entire library.

## Parameters
- `value : Any`: a variable to be checked for invalid values. If it's a collection then the function is applied recursively for all its elements.

## Returns
- `result : None`: an empty return confirming that the given value is within the extended field of real numbers.

# Examples
```Python
from mplusa import minplus as mpa
import math

try:
    print(mpa.domain.validate_domain([3.5, 1, -math.inf]))
except:
    print("This would raise an exception because of the negative infinity.")
```
