# MultivariatePolynomial
An implementation of a multivariate tropical polynomial.

## Contructor parameters
- `coefficients : numpy.ndarray`: a NumPy array representing the coefficients with each dimension being a new variable, i.e. a 2-dimensional 3x3 array would represent a polynomial of 2 variables and their combinations depending on their position in the array (the indices represent the powers in the polynomial).

## MultivariatePolynomial.\_\_call\_\_(*variables)

### Parameters
- `*variables : float`: a sequence of values within the domain to calculate the value of the polynomial for.

### Returns
- `result : float`: the value of the polynomial at the given point.

## MutlivariatePolynomial.\_\_str\_\_()

### Returns
- `result : str`: the written form of the polynomial in a form of an equation.

## MultivariatePolynomial.get_hyperplanes()

### Returns
- `result : list`: a list of linear coefficients for the hyperplanes building the polynomial.
