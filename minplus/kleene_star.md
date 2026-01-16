An implementation of Kleene star operator for tropical algebra.

$$ \mathbf{A}^{*} := \bigoplus\_{k=0}^{\infty} \mathbf{A}\_{\otimes}^{k} $$

This function does not check the convergence of the series.

Parameters
: `A : numpy.ndarray`: a square NumPy array.
: `iterations : int`: an arbitrary amount of iterations to calculate the series.

Returns
: `result : numpy.ndarray`: the resulting NumPy array.
