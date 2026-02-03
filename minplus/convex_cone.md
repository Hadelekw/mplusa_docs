An implementation of a tropical convex cone.

Constructor parameters
: `vectors : Collection[float|int]`: generators of the cone.

#### ConvexCone.get_point(constants)

Calculate a point for a given collection of constants.

Parameters
: `constants : Collection[float|int]`: a collection of constants.

Returns
: `result : numpy.ndarray`: the resulting point.

#### ConvexCone.sample_points(constants_collection)

Calculate the value of points over a grid.

Parameters
: `constants_collection : Collection[numpy.ndarray]`: collection of arguments to be exploded as arguments for numpy.meshgrid.

Returns
: `result : numpy.ndarray`: an array of points for the given grid.
