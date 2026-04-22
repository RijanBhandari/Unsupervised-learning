# Mall Customer Segmentation using K-Means Clustering

Segments mall customers into distinct groups based on Annual Income and Spending Score using K-Means clustering. Helps identify target customer profiles for marketing strategies.

## Dataset

Mall Customers dataset with 200 records and 5 features: CustomerID, Gender, Age, Annual Income (k$), and Spending Score (1-100).

## Requirements

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## What it does

**EDA** — Visualizes distribution of Gender, Age, and Annual Income using count plots.

**Feature Selection** — Uses Annual Income and Spending Score as the two clustering features.

**Elbow Method** — Runs KMeans for k=1 to 15 and plots WCSS to find the optimal number of clusters. Optimal k is 5.

**Clustering** — Fits KMeans with 5 clusters using `k-means++` initialization.

**Visualization** — Scatter plot of all 5 clusters with centroids marked.

## Results

The 5 customer segments identified:

| Cluster | Income | Spending | Profile |
|---------|--------|----------|---------|
| 1 | Low | High | Impulsive spenders |
| 2 | Medium | Medium | Balanced customers |
| 3 | High | Low | Careful high earners |
| 4 | High | High | Target customers |
| 5 | Low | Low | Budget-conscious |
