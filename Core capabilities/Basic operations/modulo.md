# modulo(a : float, t : int)
An implementation of the modulo operation in tropical algebra. Based on the definition from (Obuchowicz, D'Souza, Banaszak, 1998):

$$ \forall a,t \in [0, \infty) \exists b \in [0, \infty): a\diamond t = b \iff a = b \otimes t_{\otimes}^{k} $$
$$ \forall a \in [0, \infty): a \diamond \infty = a; \quad\forall a \in [e, \infty): \infty \diamond a = \infty $$

## Parameters
- `a : float`: a positive number within the domain.
- `t : int`: a positive integer value of the exponent.

## Returns
- `result : float`: the remainder.

# Examples
```Python
from mplusa import minplus as mpa
import math

print(mpa.modulo(10, 3))  # -> 1
print(mpa.modulo(math.inf, 8))  # -> math.inf
print(mpa.modulo(7, math.inf))  # -> math.inf
```
