An implementation of parallel composition (sum) of matrices of the same size.

$$ 
\left(\mathbf{A} \oplus \mathbf{B}\right)\_{ij} := \mathbf{A}\_{ij} \oplus \mathbf{B}\_{ij} 
$$

It is equivalent to the `numpy.minimum` function except for the validity check.

Parameters
: `A : numpy.ndarray`: a 1-dimensional or 2-dimensional NumPy array.
: `B : numpy.ndarray`: a NumPy array of the same shape as `A`.

Returns
: `result : numpy.ndarray`: a NumPy array with minimal entries.
