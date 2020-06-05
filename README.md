# Detailed Implementation of K-Means and K-Means++
This repo contains the detailed implementation of K-Means and K-Means++ clustering algorithms from scratch and an example of image Segmentation using K-Means technique.

* Showcases the comparison between the K-Means and K-Means++ technique
* Step-Wise visualization of data and clusters (using Matplotlib)
* Use of K-Means algorithm to perform image segmentation on the image - "elephant.jpg"

### K-Means Algorithm
**Input Data** : X = {x1,...,xN}

**Goal** : Partition the data among some K number of clusters. Let us assume K is known to us.

Let µk denote the center of Kth Cluster (uk will be vector)

So we need to ﬁnd an assignment of data points to clusters, as well as a set of cluster centers{µk}, such that the sum of the squares of the distances of each data point to its closest cluster center µk, is a minimum.

### K-Means++ Algorithm

K-Means is quite sensitive to initalization, if the initialization is not good, our algorithm is not able to make desired number of clusters. To overcome this problem, we use technique called K-Means++ which chooses initial centers so that they are statiscally close to final ones.

**Intuition** - Pick the centroids that are far away from one another. This increases the chances of initially picking up centroids that lie in different cluster centers. As centroids are picked from data points, each centroid has at least some data points associated with it at the end.

**Note** - Initialization is computationally more expensive in K-Means++ than the standard K-Means but the run-time for convergence to optimum is drastically reduced for K-Means++
