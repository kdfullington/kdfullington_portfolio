---
layout: page
title: "Kmeans Clustering with Health Data"
permalink: /kmeans_health/
---

[<span style="color: #FF0000; font-weight: bold;">Back to Project Page</span>](https://kdfullington.github.io/kdfullington_portfolio/projects/)

[Visit the Repository for This Project](https://github.com/kdfullington/kdfullington-portfolio/tree/main/kmeans_health_data)

For this project I performed Kmeans Clustering to categorize anonymized individuals using their health data.

I used the elbow method to determine the optimal number of K values.
![Graph](../assets/images/elbow_method_for_k.png)

I performed a silhouette analysis for several different numbers of clusters.

2 Clusters
![Graph](../assets/images/silhouette_analysis_2clusters.png)

3 Clusters
![Graph](../assets/images/silhouette_analysis_3clusters.png)


4 Clusters
![Graph](../assets/images/silhouette_analysis_4clusters.png)


5 Clusters
![Graph](../assets/images/silhouette_analysis_5clusters.png)


6 Clusters
![Graph](../assets/images/silhouette_analysis_6clusters.png)


I also made a scatterplot of the PCA transformed data, coloring each point by its cluster value. You can see that the second (PCA transformed) graph is much more orthogonal, meaning that the clusters are more distinct from each other.
![Graph](../assets/images/non_pca_scatter.png)
![Graph](../assets/images/pca_scatter.png)