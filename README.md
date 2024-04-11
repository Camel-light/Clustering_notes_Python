## Introduction to Clustering: Concepts and Code

### 01 Unsupervised Learning: An Overview
* Understanding Unsupervised Learning and its objectives
* Categories of Unsupervised Learning: 1. Clustering, 2. Association Rule, 3. Dimensionality Reduction

### 02 Clustering: An Insight
* Understanding and Applications of Clustering
* Four techniques: 1. K-Means, 2. Hierarchical, 3. DBScan, 4. Gaussian Mixture

### 03 Euclidean & Manhattan Distance: A Closer Look
* Proximity of two points indicates similarity
* Measuring distance between two points
  1. Euclidean Distance: Square root of the squared distance between two points
  2. Manhattan Distance: Absolute distance between points

### 04 K-Means Clustering: A Deep Dive
* Working of the Algorithm (Step-by-Step Computation)
* Pre-processing steps for K-Means
* How to determine the optimal number of K: 1. Profiling Approach, 2. Elbow Method

### 05 Elbow Method: A Detailed Study
* Understanding the Elbow Method with an example
* Three key concepts: 1. Total Error, 2. Variance/Total Squared Error, 3. Within Cluster Sum of Square (WCSS)

### 06 K-Means Clustering: Python Implementation
* Defining the number of clusters, selecting centroids, and measuring distance
* Euclidean Distance: Calculating the distance between points
* Determining the number of clusters using the Elbow Method
* Elbow Method: WCSS vs Number of Clusters
* Silhouette Score: Evaluating the quality of clustering

### 07 Hierarchical Clustering: An Overview
* Two Strategies: 1. Agglomerative (Bottom-Up), 2. Divisive (Top-Down)
* Types of Linkages: 
  1. Single Linkage - Nearest Neighbour (Minimum intercluster dissimilarity)
  2. Complete Linkage - Farthest Neighbour (Maximum intercluster dissimilarity)
  3. Average Linkage - Average Distance (Mean intercluster dissimilarity)
* Steps in Agglomerative Hierarchical Clustering with Single Linkage
* How to determine the optimal number of clusters: Dendrogram  

### 08 Dendrogram: A Closer Look
* Understanding the hierarchical relationship among objects
* Determining the optimal number of clusters for Hierarchical Clustering

### 09 Hierarchical Clustering: Python Implementation
* Types of Hierarchical Clustering
    1. Agglomerative: Bottom-Up approach
    2. Divisive: Top-Down approach
* Determining the number of clusters using a Dendrogram
* Dendrogram: Forming clusters based on distance and joining data points
* Linkage: Calculating the distance between two points in two clusters
    1. Single linkage: Minimum distance between two clusters
    2. Complete linkage: Maximum distance between two clusters
    3. Average linkage: Average distance between two clusters

### 10 DBScan Clustering: An Overview
* Density-Based Clustering
* K-Means & Hierarchical are suitable for compact and well-separated data
* Both are sensitive to outliers and noise
* DBScan addresses these issues and handles outliers effectively
* Two crucial parameters - 
  1. eps: If the distance between two points is less than or equal to eps, they are considered neighbours
  2. MinPts: Minimum number of neighbours/data points within eps radius

### 11 DBScan Clustering: Python Implementation
* No need to predefine clusters
* The distance metric used is Euclidean Distance
* Two parameters are required
    1. eps: Radius of the circle
    2. min_samples: Minimum data points to form a cluster

### 12 GMM Clustering: An Overview
* Limitations of K-Means
* Expectation Maximization (EM) method

### 13 Gaussian Mixture Model Clustering: Python Implementation
* Probabilistic Model
* Utilizes Expectation-Minimization (EM) steps:
    1. E Step: Calculating the probability of each data point for each cluster
    2. M Step: Revising parameters based on probability for each cluster

### 14 Cluster Adjustment: An Overview
* Two common steps for Cluster Adjustment 
  1. Evaluating the quality of clustering (Cardinality & Magnitude)
  2. Assessing the performance of the similarity measure (Euclidean Distance)

### 15 Silhouette Coefficient - Cluster Validation: An Overview
* Clusters are well separated if the silhouette score is closer to 1
* It is a measure used to assess the quality of a clustering technique 
* Its value ranges from -1 to 1.
    1. 1: Indicates that clusters are well separated from each other
