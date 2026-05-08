# draw_polytope2D(...)
Draws a polytope on a 2D plot.

## Parameters
- `polytope : AbstractPolytope`: a 2-dimensional `AbstractPolytope`.
- `color : str`: the color to render the edges of the polytope with. Defaults to `black`.
- `show_vertices : bool`: whether or not to show vertices of the polytope. Defaults to `True`.
- `vertices_color : str|None`: the color to render the vertices with. Defaults to `None` which will cause it to draw with the default `color` parameter.
- `vertices_marker : str`: the marker to render the vertices with. Defaults to `o`.
- `show_pseudovertices : bool`: whether or not to show pseudovertices of the polytope. Defaults to `False`.
- `pseudovertices_color : str|None`: the color to render the pseudovertices with. Defaults to `None` which will cause it to draw with the default `color` parameter.
- `pseudovertices_marker : str`: the marker to render the pseudovertices with. Defaults to `o`.
- `show : bool`: whether or not to invoke `matplotlib.pyplot.show` at the end.
