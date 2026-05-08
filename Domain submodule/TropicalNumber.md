# TropicalNumber
An empty class inheriting from metaclass `TropicalNumberMeta`. It has overwritten \_\_instancecheck\_\_ which allows for validation of any value against this class using isinstance.

# Examples
```Python
from mplusa import minplus as mpa
import math

print(isinstance(3.89, mpa.domain.TropicalNumber))  # -> True
print(isinstance(-math.inf, mpa.domain.TropicalNumber))  # -> False
```
