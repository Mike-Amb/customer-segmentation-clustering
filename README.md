# Mall Customer Segmentation

Unsupervised machine learning project applying K-Means and Hierarchical Clustering to segment mall customers based on spending behavior, income, and demographics. The goal is to identify distinct customer groups that can inform targeted marketing strategies.

## Dataset

Source: [Kaggle - Customer Segmentation Tutorial](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

200 mall membership card holders with features: Age, Annual Income, and Spending Score.

## Methodology

**K-Means Clustering** — primary method with optimal cluster count determined by the Elbow Method and validated using the Silhouette Score.

**Hierarchical Clustering** — secondary method used to independently confirm the cluster structure via dendrogram analysis.

Both methods converged on five segments with an Adjusted Rand Index of 0.942, confirming the robustness of the segmentation.

## Customer Segments

| Cluster | Profile | Size |
|---|---|---|
| 0 | Average Income, Average Spend | 81 |
| 1 | High Income, High Spend | 39 |
| 2 | Low Income, High Spend | 22 |
| 3 | High Income, Low Spend | 35 |
| 4 | Low Income, Low Spend | 23 |

Cluster 3 represents the highest untapped revenue opportunity — customers with the means to spend but who are not converting.

## Dependencies

```
pandas
numpy
matplotlib
seaborn
scikit-learn
scipy
```

## Data Source

Kaggle — vjchoudhary7/customer-segmentation-tutorial-in-python
