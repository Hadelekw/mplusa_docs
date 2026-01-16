An implementation of multiple multiplication on a matrix. By definition from [^1]:

$$ 
\exists k_0 \forall k \geq k_0: \mathbf{A}\_{\otimes}^{k + 1} := \mathbf{A}\_{\otimes}^{k} 
$$ $$
\mathbf{A}\_{\otimes}^{k} = \mathbf{A} \otimes \mathbf{A}\_{\otimes}^{k - 1}, \quad \mathbf{A}\_{\otimes}^{0} = \mathbf{E}
$$

with E being a tropical unit matrix. It applies if A is a matrix with non-negative entries and its diagonal elements are equal to the tropical identity element.

Parameters
: `A : numpy.ndarray`: a square NumPy array.
: `k : int`: an integer value of the exponent.

Returns
: `result : numpy.ndarray`: a square NumPy array.
