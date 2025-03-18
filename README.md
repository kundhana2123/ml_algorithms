# ml_algorithms

# K-Means Clustering
The dataset used in the code can be downloaded from the kaggle website which can be found [here](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python?select=Mall_Customers.csv).
## Overview:
K-Means Clustering is an unsupervised machine learning algorithm used to partition a dataset into k distinct clusters based on similarity. Each cluster contains data points that are closer to the corresponding cluster centroid compared to others.

## Goals of K-Means Clustering:
1. Identify hidden patterns within the data.
2. Summarize the data using cluster centroids, which represent the center of each cluster.
3. Dimensionality reduction: One-hot encoding or feature selection can be applied to reduce feature space.
## Key Concepts:
1. k represents the number of clusters.
2. The optimum value of k is not known initially and needs to be determined using methods like the Elbow Method or Silhouette Score.
3. Initially, the cluster membership is unknown, and the algorithm assigns points to clusters iteratively.
## Working of K-Means Clustering:
1. Randomly select k points: These points will act as the initial centroids of the clusters.
2. Assign each data point to the nearest centroid based on distance (usually Euclidean distance).
3. Recalculate each centroid: Update the centroid by calculating the mean of all data points assigned to it.
4. Repeat steps 2 and 3: Continue until the centroids do not change significantly or the maximum number of iterations is reached.
## Objective Function:
The objective function for K-Means is WCSS (Within-Cluster Sum of Squares), which minimizes the sum of squared distances (J) between each point and its assigned centroid. This ensures the points within each cluster are as close as possible to the centroid.
## How to Calculate the Number of Clusters (k)?


Determining the optimal number of clusters can be challenging. Popular techniques to calculate k include:
1. Elbow Method: Plot the WCSS values for different values of k and look for an "elbow" point where the reduction in WCSS starts to slow down.
2. Silhouette Score: Measures how similar each point is to its own cluster compared to other clusters.
## Challenges and Limitations:
1. Different initial centroids can lead to different results (local minima).
2. K-Means assumes clusters are spherical, which may not work well for clusters with complex or elongated shapes.
3. Outliers can distort the mean-based centroid calculation, leading to inaccurate clusters.
4. Sensitive to the choice of k: The algorithm may not perform well if k is not chosen properly.
## Applications:
1. Market segmentation: Grouping customers based on spending patterns or preferences.
2. Image compression: Reducing the number of colors in an image by clustering similar colors together.
3. Document clustering: Grouping documents with similar topics or content together.
