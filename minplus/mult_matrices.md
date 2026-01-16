An implementation of series composition (product) of matrices of sizes MxN and NxP.

$$ 
\left(\mathbf{A} \otimes \mathbf{B}\right)\_{ij} := \bigoplus\_{k=1}^{N}\left(\mathbf{A}\_{ik} \otimes \mathbf{B}\_{kj}\right)
$$

Parameters
: `A : numpy.ndarray`: a NumPy array of shape MxN.
: `B : numpy.ndarray`: a NumPy array of shape NxP.

Returns
: `result : numpy.ndarray`: a NumPy array of shape MxP.
