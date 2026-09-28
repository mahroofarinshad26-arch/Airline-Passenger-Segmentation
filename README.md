# Airline-Passenger-Segmentation


##  Project Overview

This project focuses on segmenting airline passengers into meaningful groups using unsupervised machine learning techniques.

The Airline Passenger Satisfaction dataset is analyzed using different clustering algorithms to identify hidden patterns and similarities among passengers based on their demographic, travel, flight, and service-related features.

##  Objective

The main objective of this project is to identify meaningful passenger segments using clustering techniques and compare different unsupervised learning algorithms.

##  Dataset

- Dataset: Airline Passenger Satisfaction
- Number of Records: 103,904
- Original Features: 25
- Target/Label: Satisfaction
- The `satisfaction` column was excluded from clustering because this is an unsupervised learning project.

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

##  Project Workflow

1. Data Collection and Loading
2. Data Understanding
3. Exploratory Data Analysis
4. Missing Value Handling
5. Duplicate Checking
6. Outlier Detection and Treatment
7. Feature Selection
8. Categorical Encoding
9. Feature Scaling
10. Elbow Method
11. K-Means Clustering
12. Hierarchical Clustering
13. DBSCAN Clustering
14. PCA Visualization
15. Cluster Evaluation
16. Algorithm Comparison
17. K-Means Model Saving


##  Clustering Algorithms

### 1. K-Means Clustering

K-Means clustering was used to divide passengers into 4 clusters based on similarities between their features.

### 2. Hierarchical Clustering

Hierarchical Clustering was applied to identify passenger groups using an agglomerative clustering approach.

### 3. DBSCAN

DBSCAN was used to identify dense passenger groups and detect noise points.

##  Evaluation Metrics

The clustering algorithms were evaluated using:

- Elbow Method
- Silhouette Score
- Davies-Bouldin Index

##  Results

| Algorithm | Silhouette Score | Davies-Bouldin Index |
|-----------|------------------|----------------------|
| K-Means | 0.1022 | 2.4256 |
| Hierarchical | 0.0856 | 2.5480 |
| DBSCAN | 0.0099 | 3.7868 |

Based on the obtained evaluation metrics, K-Means produced the comparatively better clustering result among the evaluated methods.

## 📈 Visualizations

The project includes:

- Categorical Count Plots
- Age Distribution
- Flight Distance Distribution
- Box Plots
- Correlation Heatmap
- Elbow Method Plot
- PCA Cluster Visualizations
- Clustering Performance Comparison

##  Key Insights

- Four passenger segments were identified using K-Means.
- The clusters differ in terms of passenger age, flight distance, and service ratings.
- Cluster 1 has the highest average flight distance and generally higher service ratings.
- Cluster 2 contains younger passengers and has a lower average flight distance.
- The four clusters have relatively balanced sizes.

##  Model Saving

The trained K-Means model was saved using Joblib.

File:

`airline_kmeans_model.pkl`

##  Conclusion

This project demonstrates how unsupervised machine learning can be used to discover meaningful passenger segments without using predefined target labels.

K-Means, Hierarchical Clustering, and DBSCAN were applied and evaluated using different clustering evaluation metrics. The analysis provides useful insights into different passenger groups based on their travel and service-related characteristics.

