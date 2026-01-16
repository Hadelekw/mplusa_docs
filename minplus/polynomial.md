(inherits from *MultivariatePolynomial*)

An implementation of a single-variable tropical polynomial.

Contructor parameters
: `*coefficients : float`: values to be used as the coefficients.

#### Polynomial.get_line_intersections()

Returns
: `result : list`: a list of points where the lines building the polynomial intersect.

#### Polynomial.get_roots()

Returns
: `roots : list`: a list of the roots' values.
: `ranks : list`: a list of the corresponding ranks (amount of monomials attaining the value).
