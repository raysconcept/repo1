# Test task

whole task is to create animated spline wave using shaders

1. Clone this source and put it somewhere online (for instance <username>.github.io/some.html), make it working.

1. change  createMyCustomGeometry, which is easy to manipulate for spline functions: It must be rectangular face with properties:
   * have N-width segments.
   * Have only one height segment;
   * `x` increases from `0,0` to `1.0` 
   * `y` could be `-1.0` or `1.0`
   * must have UV coordinates;
   * Geometry must be instance of `THREE.Geometry`

   for `N == 3` we will have set of vertices = `[(0,1), (0.5, 1), (1.0, 1), (0, -1), (0.5, -1), (1.0, -1)];`

2. Create array of positions that forming some kind of time-based waving. Create array of matrices, according to this positions and pass it to shader program as uniform value
3. Implement multipoint spline in shader:
    ![Spline Formula](/textures/spline.jpg)

4. Draw spline on current canvas, using your shader and geometry, your have create, textured with earth texture.
5. Make texture slowly moving along your spline width.

That's it.


