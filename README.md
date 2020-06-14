## Voronoi 3D Object
The Voronoi diagram is the decomposition of a space into polygonal partitions. For any set of objects in a two or three dimensional space, a polygonal shape surrounds the object such that approximately any point in the polygon is closer to its generated object than any other generated object. Even tough its definition may seem elaborated this pattern is very common to see in natural environment like the giraffe’s fur, the veins on a dragonfly’s wings, the honeycomb cells built by bees and even in human skin.

In order to create a Voronoi mesh a set of randomly distributed points is needed. The distribution of the set of points is not really important, and actually playing around with this distribution can create very interesting patterns. Once the set of points is defined the Delaunay triangulation is computed, which is basically connecting the points to the closest neighboring points. Then the center of the circumcircles of each triangle is computed and connected to the ones on adjacent triangles. Finally the infinite edges that extend from the convex hull are also computed.

Once the Voronoi vectors are computed, these can be used to create a mesh to form a specific shape like an icosahedron with ThreeJS.

[DEMO](https://jaec86.github.io/amt-workshop3/)
