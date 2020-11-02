# Makogan

I am a computer scientist focused on computer graphics. I really like research and learning and want to be a full time researcher in computer graphics.

Currently I am making my own rendering engine, focused on making research prototypes as easy as possible.

However you should also take a look at [my old projects](/projects.md).

You should also check [my proof repository](https://gitlab.com/Makogan/mathproofs) where I have proven some facts about papers and algorithms I am interested about, my favourites are the proofs on b splines and the proofs on gaussian subdivision.


## Engine highlights

These are some neat algorithms I have implemented in my current engine, which is made with Vulkan and C++.


### Gaussian Subdivision

Gaussian subdivision is a 2019 SIGGRAPH paper, it is a generalization of subdivision surfaces using gaussian distributions at every point.

This is a guassian loop subdivided bunny where the gaussian distributions at the vertices where randomly generated.

![bunny](/images/gaussian_bunny.png)

This is a guassian loop subdivided cube where only one of the vertices has a non identity gaussian matrix.

![cube](/images/gcube.png)

### Polyhedral Exact Geodesics

I have a partial implementation of the MMP algorithm for exact geodesics (coded entirely by me):

![bunny](/images/bunny1.png)
![bunny](/images/bunny2.png)
![bunny](/images/bunny3.png)
![bunny](/images/bunny4.png)
![bunny](/images/bunny5.png)

### Half edge data structure with boundary

I have an efficient implementation fo the half edge data structure that handles boundary conditions. The above algorithms both use this data structure, but since they don't have boundaries, here is an example of regular loop subdivision in a tetrahedron missing one face:

![bunny](/images/boundary_condition.png)