To properly implement Skybox, the sky needs to use its own
pipeline and shaders. This will look the same as the last 
tutorial, but it will warm us up for more difficult tutorials
that require more pipelines: lighting, particles, etc

We add the shaders sky.vert and sky.frag, which are similar
to cube.vert and cube.frag, except cube.vert sets the pixels
of the skybox to the maximum depth. 

Sky.frag takes the texture of the color, and puts it on
the screen. Cube.frag multiplies the color by ambient
occlusion, to darken the pixels. This gives us room to
implement lighting. Also, the ambient lighting matches
the skybox, for a cool effect

