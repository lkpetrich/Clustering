# Clustering
Finds clustering of entities.

**File: Distance-Matrix Cluster Analysis.nb - Mathematica**

Implements several algorithms for finding clustering from distance matrices.
Each entry in a distance matrix is the distance between two entities.
* Multidimensional scaling: finds positions of points where the distance between each pair of them is the value of the distance-matrix entry for them.
* K-Medoids: like k-means, but instead uses a median-like algorithm.
* Neighbor joining: algorithms for building a clustering tree by repeatedly finding the closest neighbor to a partial tree and then adding it to that tree.
  * WPGMA -- Weighted Pair Group Method with Arithmetic Mean
  * UPGMA -- Unweighted Pair Group Method with Arithmetic Mean
  * SingleLink - single-linkage clustering
  * CompleteLink - complete-linkage clustering
  * NeiSaitou - Nei-Saitou neighbor joining
  * BIONJ - modification of NS algorithm
* Fitch-Margoliash Fitting: given a tree and a distance matrix, what are the best-fitting branch lengths?
* Fitch-Margoliash Building: random trees, assembling a tree with the best fit for each new entry, and flipping branches in the tree to find improved fits.

**File: Distance-Matrix Cluster-Analysis Tests.nb - Mathematica**

Has tests of most of these algorithms.
