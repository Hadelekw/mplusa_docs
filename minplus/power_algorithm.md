An algorithm for calculating the eigenvalue of a irreducible matrix, as defined in [^3]. This function does not check for the matrix reducibility and therefore may return wrong results in some cases.

Parameters
: `A : numpy.ndarray`: a NumPy array representing the matrix.
: `x_0 : numpy.ndarray|None`: a vertical NumPy vector; initial guess for which the next step will be calculated. If it's equal to None then it is assumed to be a vertical vector of ones. Defaults to None.
: `iterations : int`: the maximum numbers of iterations to calculate the power series. Defaults to 1000.

Returns
: `p : int`: one of the values necessary for the calculations of the eigenvalue (see above).
: `q : int`: one of the values necessary for the calculations of the eigenvalue (see above).
: `c : float`: one of the values necessary for the calculations of the eigenvalue (see above).
: `xs : list`: history of the vectors calculated during the search.
