Generates a two dimensional tropical unit matrix. In the (min, +) version it is defined as:

$$
\mathbf{E}_{ij} := \begin{cases} 0, &i = j\\ \infty, &i \neq j \end{cases}
$$

Parameters
: `width : int`: the width of the unit matrix.
: `height : int`: the height of the unit matrix.

Returns
: `result : numpy.ndarray`: a NumPy array tropcial unit matrix.
