# Customer Segmentation with Clustering
### E-Commerce Transnational Dataset | Cambridge Data Science Programme

A customer segmentation analysis for a transnational e-commerce 
company spanning 47 countries across 5 continents. Built to support 
more targeted marketing strategies through unsupervised machine 
learning.

---

## Problem

An e-commerce company with 951,669 transactions needed to understand 
its customer base and improve marketing efficiency through meaningful 
customer segmentation.

---

## Approach

Five features were derived through feature engineering from 20 raw 
variables: **Frequency, Recency, Average Unit Cost, Customer Lifetime 
Value (CLV) and Age.**

| Method | Type | Purpose |
|--------|------|---------|
| K-Means Clustering | Unsupervised ML | Primary segmentation model |
| Hierarchical Clustering | Unsupervised ML | Validate cluster count |
| Elbow Method | Evaluation | Determine optimal k |
| Silhouette Score | Evaluation | Validate cluster quality |
| PCA + t-SNE | Dimensionality Reduction | Visualise clusters |

---

## Key Findings

- **5 clusters** identified as optimal across all three evaluation 
  methods (Elbow, Silhouette, Dendrogram)
- **Cluster 4**: high frequency, high CLV, low recency, active 
  customers. Recommended: reward and referral programmes
- **Cluster 1**: high recency, low engagement, at-risk customers. 
  Recommended: targeted re-engagement offers
- Silhouette score of 0.267 at n=5 - best separation achieved
- t-SNE at perplexity=15 produced the tightest, most differentiated 
  cluster visualisation

---

## Methods
```python
# Core libraries
sklearn.cluster      # KMeans, AgglomerativeClustering
sklearn.metrics      # silhouette_score
sklearn.decomposition # PCA
sklearn.manifold     # TSNE
```

---

## Author

**Israel Olujobi**  
Cambridge Data Science & AI Programme (December 2025)
