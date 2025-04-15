# Clustering Analysis on Air Quality Dataset

This project performs clustering analysis on the [UCI Air Quality dataset](https://archive.ics.uci.edu/ml/datasets/Air+Quality), evaluating the effectiveness of various preprocessing techniques and clustering algorithms.

## Dataset Overview

The dataset contains sensor readings of various gas concentrations and environmental factors collected over time. Preprocessing was necessary to handle missing values and prepare the data for clustering.

---

## Clustering Methods Used

- **KMeans**
- **Hierarchical (Agglomerative) Clustering**
- **Mean Shift Clustering**

---

## Preprocessing Techniques

We tested clustering with the following transformations:

- No processing (raw features)
- Normalization
- Transformation
- PCA (2 components)
- Transformation + Normalization
- Transformation + Normalization + PCA

---

## Evaluation Metrics

Each clustering was evaluated using:

- **Silhouette Score** – measures cohesion vs. separation
- **Calinski-Harabasz Index** – ratio of dispersion between and within clusters
- **Davies-Bouldin Score** – lower is better, indicates tighter clustering

---

## Key Insights

- KMeans performed consistently well across all preprocessing strategies.
- PCA improved clustering performance across all algorithms.
- Mean Shift was sensitive to preprocessing and bandwidth, sometimes producing only one cluster.
- T+N+PCA generally provided the best overall performance.

---

## Repository Structure

- notebook.ipynb – Jupyter Notebook with complete analysis and result tables
- README.md – This file with project summary and key findings

---

## Conclusion

Clustering effectiveness is highly influenced by preprocessing. KMeans with PCA showed the strongest results for the Air Quality dataset.

---

## References

- UCI Machine Learning Repository: Air Quality Dataset
- Scikit-learn Documentation
