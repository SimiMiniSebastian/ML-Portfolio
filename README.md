# ML-Portfolio
Comparison of K-Means and Hierarchical Clustering on Multiple Datasets
This project demonstrates the implementation and comparison of two clustering algorithms, K-Means and Hierarchical Clustering, on three datasets: Iris, Moons, and Blobs. The project focuses on clustering real-world and synthetic datasets and evaluates the performance of each algorithm using metrics such as Silhouette Score, Cluster Purity, and Execution Time.

1. Project Introduction & Data Selection
We utilize the following datasets:

Iris Dataset: A classic dataset with 3 clusters, each corresponding to a species of iris flowers. This is used as an example of high-dimensional data (4D).
Moons Dataset: A synthetic dataset with 2 clusters in a non-linearly separable arrangement. This is a 2D dataset used to study the performance of clustering on complex, non-linear structures.
Blobs Dataset: A synthetic dataset with 3 clusters and varying densities. This is used for studying density variations in clusters.
Each dataset is scaled using StandardScaler for normalization.

2. K-Means Clustering Implementation
We implement K-Means Clustering on all three datasets:

Iris Dataset: We applied K-Means with 3 clusters.
Moons Dataset: We applied K-Means with 2 clusters.
Blobs Dataset: We applied K-Means with 3 clusters.
For each dataset, the Silhouette Score is calculated to evaluate the quality of clustering.

3. Hierarchical Clustering Implementation
We implement Hierarchical Clustering (Agglomerative Clustering) on the same datasets:

Iris Dataset: Hierarchical Clustering with 3 clusters.
Moons Dataset: Hierarchical Clustering with 2 clusters.
Blobs Dataset: Hierarchical Clustering with 3 clusters.
Similarly, Silhouette Scores are calculated for comparison.

4. Visualizations
For each dataset, we visualize the clusters formed by both K-Means and Hierarchical Clustering:

Iris Dataset: 3D visualization using the first 3 features.
Moons Dataset: 2D visualization.
Blobs Dataset: 2D visualization using PCA to reduce dimensionality to two components.
5. Comparison Between K-Means and Hierarchical Clustering
5(a) Execution Time:
We measure the time taken by each algorithm to cluster the Iris dataset, highlighting the computational efficiency of each method.

5(b) Cluster Purity:
We calculate Cluster Purity for both algorithms to assess how well the clusters match the true class labels in the Iris Dataset.

Results
Dataset	Algorithm	Silhouette Score	Execution Time (s)	Cluster Purity
Iris	K-Means	0.55	0.03	0.89
Hierarchical	0.48	0.05	0.85
Moons	K-Means	0.50	0.02	-
Hierarchical	0.49	0.04	-
Blobs	K-Means	0.70	0.02	-
Hierarchical	0.63	0.04	-
6. Conclusion
K-Means generally performs better in terms of Silhouette Score and Execution Time, especially for linearly separable datasets like Blobs.
Hierarchical Clustering offers a good alternative, especially for smaller datasets, and is more intuitive for non-linearly separable datasets like Moons.
Cluster Purity results show that both methods can effectively separate clusters, though K-Means slightly outperforms Hierarchical Clustering on the Iris dataset.
