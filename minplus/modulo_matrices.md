An implementation of the modulo operation for matrices according to [^1]. If A is an MxN matrix with non-negative entries and b is an m-element vector with non-negative entries, then B is an MxN matrix defined by:

$$ 
\mathbf{B}\_{ij} := \mathbf{A}\_{ij} \diamond \mathbf{b}\_{i} 
$$

Parameters
: `A : numpy.ndarray`: a NumPy array.
: `b : numpy.ndarray`: a vertical NumPy array of size Mx1.

Returns
: `result : numpy.ndarray`: a NumPy array of remainders.
