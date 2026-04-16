# 🌸 Iris Clustering with DBSCAN

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Machine Learning](https://img.shields.io/badge/ML-Unsupervised-orange.svg)
![Algorithm](https://img.shields.io/badge/DBSCAN-Clustering-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📌 Overview

This project applies **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** to the classic Iris dataset to identify natural groupings of flowers without using labels.

Unlike K-Means, DBSCAN does not require predefining the number of clusters and can detect **noise (outliers)**.

---

## 🎯 Objective

- Cluster Iris flowers using sepal and petal measurements  
- Identify natural density-based groupings  
- Detect outliers in the dataset  
- Compare results with true species labels  

---

## ⚙️ Workflow

### 1. Data Preparation
- Loaded Iris dataset from `scikit-learn`
- Applied **StandardScaler** for feature normalization

### 2. Parameter Selection
- Used **k-distance plot (5th nearest neighbor)**
- Selected optimal **ε (epsilon)** using the elbow method

### 3. DBSCAN Clustering
- Applied `DBSCAN` from `scikit-learn`
- Assigned cluster labels and identified noise points (`-1`)

### 4. Evaluation
- **Silhouette Score** → cluster cohesion & separation  
- **Adjusted Rand Index (ARI)** → comparison with true labels  

---

## 📊 Results

- **Silhouette Score:** ~0.60  
- **Adjusted Rand Index:** ~0.54  

### Key Insight:
DBSCAN successfully identified meaningful clusters but shows partial overlap between Iris species due to natural feature similarity.

---

## 🧰 Tech Stack

- Python 🐍  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Scikit-learn  

---

## 📁 Project Structure

Iris.ipynb # Main notebook (data preprocessing, clustering, visualization)
README.md # Project documentation

---

## 📈 Key Learnings

- DBSCAN does not require predefined cluster numbers  
- Feature scaling is critical for distance-based clustering  
- ε selection strongly impacts results  
- Iris dataset is only partially density-separable  

---

## 🚀 Future Work

- Compare DBSCAN with K-Means and Hierarchical clustering  
- Apply PCA for better visualization  
- Experiment with different `min_samples` values  
- Automate epsilon tuning methods  

---

## 👤 Author

Unsupervised learning project based on the Iris dataset using DBSCAN for clustering and anomaly detection.