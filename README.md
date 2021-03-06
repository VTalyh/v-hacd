# v-hacd
The V-HACD library decomposes a 3D surface into a set of "near" convex parts
![Alt text](/snapshots/acd.png)
## Why do we need approximate convex decomposition?
Collision detection is essential for [realistic physical interactions](https://www.youtube.com/watch?v=oyjE5L4-1lQ) in video games and computer animation. In order to ensure real-time interactivity with the player/user, video game and 3D modeling software developers usually approximate the 3D models composing the scene (e.g. animated characters, static objects...) by a set of simple convex shapes such as ellipsoids, capsules or convex-hulls. In practice, these simple shapes provide poor approximations for concave surfaces and generate false collision detection.
![Alt text](/snapshots/chvsacd.png)
A second approach consists in computing an exact convex decomposition of a surface S, which consists in partitioning it into a minimal set of convex sub-surfaces. Exact convex decomposition algorithms are NP-hard and non-practical since they produce a high number of clusters. To overcome these limitations, the exact convexity constraint is relaxed and an approximate convex decomposition of S is instead computed. Here, the goal is to determine a partition of the mesh triangles with a minimal number of clusters, while ensuring that each cluster has a concavity lower than a user defined threshold.

![Alt text](/snapshots/ecdvsacd.png)
# More approximate convex decomposition results
![Alt text](/snapshots/snapshots_1.png)
![Alt text](/snapshots/snapshots_2.png)
![Alt text](/snapshots/snapshots_3.png)
![Alt text](/snapshots/snapshots_4.png)
![Alt text](/snapshots/snapshots_5.png)
