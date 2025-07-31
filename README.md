# Clustering Lab Report  
**Author**: Shashwat Baral  
**Course**: Principles of Cybersecurity  
**Lab Topic**: Clustering Analysis and Data Exploration  

---

## 🔍 Purpose of the Lab

The aim of this lab was to implement unsupervised machine learning methods—specifically clustering—to examine a dataset that includes global internet usage statistics. Through exploratory data analysis (EDA), dimensionality reduction, and clustering techniques such as K-Means, I sought to uncover hidden patterns and groupings within the data. This practical exercise reinforced essential concepts in cybersecurity analytics and machine learning processes.

---

## 💡 Key Insights from Clustering Results and Visualizations

- **Optimal Clusters**: By employing the Elbow Method and Silhouette Score, I concluded that 3 to 5 clusters effectively represented the data's structure. I opted for 4 clusters to achieve a balance between accuracy and simplicity.
  
- **Country Groupings**: Nations with comparable rankings and data usage trends were naturally clustered together, frequently corresponding with geopolitical and economic regions.
  
- **Principal Component Analysis (PCA)**: Reducing the data to two dimensions via PCA facilitated effective visualization of the cluster separations. It indicated that certain features (such as ranking and region) significantly impacted clustering.
  
- **Feature Relationships**: Ranking, date of information, and internet usage values emerged as crucial factors influencing cluster membership.

---

## ⚠️ Challenges and Decisions Made

- **High Dimensionality**: The dataset contained over 600 one-hot encoded columns. To address this, I utilized PCA to reduce dimensionality while maintaining variance.
  
- **Target Confusion**: At first, I presumed a 'Data Usage (MB)' target column was present. However, the dataset did not include a numeric target, prompting me to transition to an unsupervised methodology instead.
  
- **Sparse Categorical Data**: Numerous countries and values resulted in sparse binary columns post-encoding. This issue was alleviated by eliminating redundant features and scaling the data using `StandardScaler'.
  
- **Selecting the Appropriate Number of Clusters**: Determining the value of `k` for KMeans necessitated iterative experimentation utilizing both visual (elbow plot) and metric-based (silhouette score) methods.

---

## 📁 Directory Structure

- `clustering_lab.ipynb` – The primary notebook encompassing all procedures: loading, preprocessing, clustering, and visualization.
- `README.md` – This document provides a summary of the lab's objectives, results, and reflections.
---

## ✅ Summary

This laboratory exercise enhanced my comprehension of unsupervised learning, particularly how KMeans and PCA can reveal patterns within intricate datasets. Clustering serves as a robust tool in cybersecurity for anomaly detection, user segmentation, and classification of threat groups. This practical experience underscored the significance of data preparation, evaluation metrics, and the interpretability of models.
