An implementation of the addition operation in tropical algebra.

$$
\forall a, b \in \mathbb{R}_{\min}: a \oplus b := \min\{a, b\} 
$$

It is equivalent to the `min` function except for the validity check.

Parameters
: `*args : float`: numerical arguments within the domain.

Returns
: `result : float`: the minimum.
