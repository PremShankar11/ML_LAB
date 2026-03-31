
# Experiment 8: Clustering Human Activity Recognition Data

## Name: PREM SHANKAR.S

## RegNo: 3122235001101

## 📌 Objective
To implement and compare K-Means, DBSCAN, and Hierarchical Clustering on the Human Activity Recognition (HAR) dataset and evaluate their performance using various metrics.

---

## 📂 Dataset
The UCI HAR dataset contains sensor data from smartphones for 6 human activities, preprocessed into feature vectors of 561 attributes.

---

## 🔧 Step 1: Data Loading
Loaded training and testing datasets, combined them, and assigned feature names and activity labels for a complete dataset.

---

## 🧹 Step 2: Preprocessing
Checked for missing values and applied standardization to ensure all features contribute equally to distance-based clustering.

---

## 📉 Step 3: Dimensionality Reduction (PCA)
Reduced high-dimensional data to 2 principal components for visualization while retaining significant variance.

---

## 🔵 Step 4: K-Means Clustering
Applied K-Means for k = 2 to 8, computed WCSS and Silhouette scores, and selected the optimal k using Elbow and Silhouette methods.

---

## 🟣 Step 5: DBSCAN Clustering
Used k-distance graph to determine eps and applied DBSCAN to identify clusters and detect noise points.

---

## 🟢 Step 6: Hierarchical Clustering
Performed Agglomerative clustering with Ward linkage and used a dendrogram to determine the number of clusters.

---

## 📊 Step 7: Evaluation Metrics
Evaluated all models using internal metrics (Silhouette, Davies-Bouldin, Calinski-Harabasz) and external metrics (ARI, NMI).

---

## 📈 Step 8: Visualization & Comparison
Visualized clusters using PCA plots and compared algorithm performance using bar charts and scatter plots.

---

## ✅ Conclusion
K-Means performed best overall, DBSCAN effectively detected noise but struggled with high dimensions, and Hierarchical clustering provided structured insights but at higher computational cost.

