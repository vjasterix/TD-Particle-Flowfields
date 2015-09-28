# Particle-Flowfields-Touchdesigner

> Licensed under Creative Commons Attribution-NonCommercial. Please request permission if you would like to use for commercial applications.

***

![preview here](https://i.vimeocdn.com/video/519057929_295x166.webp)
[See example on my vimeo feed](https://vimeo.com/128060350)

# What is it?
This demonstrates a technique of performing particle calculations inside textures, which has significant performance benefits over cpu methods, allowing users to create several million particles really easily. Turbulence is added into the scene using vector flowfield like behaviours, as well as some curling effects which are probably more noticable

# Usage
Documentation is noted throughout the tox file in little text DATs and also within the pixel shaders. 

#Different Geometry
You can feed in other geometry as an emitter source (plug it into finalGeo null)  so long as: its vertex count is the same or less as particle count chop ( 500 verts).

#More Particles
Currently the demo is rigged so you just need to increase the particle count chop to get more particles. It is the square root of the final particles produced. 
However I'm sure you'll want to play with different meshes so keep ing mind:
You can increase the number of particles in the current sketch by increasing the particle count chop, which is the square root of the total particles emmitted. ie set it to 500 an your particles will be 250,000. set it to 1000 and your particles will be 1,000,000
Keep in mind your finalGeo sop must have the same amount of particles as particlecount. And particles SOP's vertices has the final amount of particles.

#Different Displacement Textures
Try patching in some geometric textures to nx and nx1 for interesting effects.

# Have fun
Please experiment and read through the notes so you can learn and make similar cool things. I won't be offering support however I am available to hire for commercial projects.

