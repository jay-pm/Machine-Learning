

## K-means

**Basics:**
- The KMeans algorithm clusters data by trying to separate samples in n groups of equal variance, minimizing a criterion known as the inertia or within-cluster sum-of-squares.
- This algorithm requires the number of clusters to be specified.
- It scales well to large number of samples and has been used across a large range of application areas in many different fields.
- K-means is often referred to as Lloyd’s algorithm

**How it works:**

- Chooose random number of centroids
- Assign each sample to it's nearest centroid. Distance metric: Euclidean
- Calculate new centroids by taking the mean value of all of the samples assigned to each previous centroid.
- Repeat step 2 and 3 until the centroids do not move significantly.
- k-means++ initialization scheme: This initializes the centroids to be (generally) distant from each other, leading to probably better results than random initialization.
A parameter can be given to allow K-means to be run in parallel, called n_jobs. Giving this parameter a positive value uses that many processors (default: 1). A value of -1 uses all available processors, with -2 using one less, and so on. Parallelization generally speeds up computation at the cost of memory (in this case, multiple copies of centroids need to be stored, one for each job).

**Evaluation:**

- The Silhouette Coefficient is calculated using the mean intra-cluster distance (a) and the mean nearest-cluster distance (b) for each sample.
- The Silhouette Coefficient for a sample is (b - a) / max(a,b). b is the distance between a sample and the nearest cluster that the sample is not a part of.
- The best value is 1 and the worst value is -1.
- Values near 0 indicate overlapping clusters.
- Negative values generally indicate that a sample has been assigned to the wrong cluster, as a different cluster is more similar.
