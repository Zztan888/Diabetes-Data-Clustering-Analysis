# 🧪 Diabetes Data Clustering Analysis

This repository contains an implementation of a Clustering algorithm to analyze patterns in the **Diabetes Dataset**. This project was completed as part of Assignment 2.

---

## 📑 Project Components
* **Algorithm:** K-Means Clustering
* **Language:** Python (Jupyter Notebook)
* **Dataset:** `diabetes.csv`

---

## 📂 Quick Links to Files
* 📄 **Full Report:** [Report_for_clustering_A2.pdf](./Report_for_clustering_A2_git.pdf)
* 📓 **Source Code:** [Assignment2.ipynb](./Assignment2.ipynb)
* 📊 **Dataset:** [diabetes.csv](./diabetes.csv)

---

## 🤖 Algorithm Introduction: K-Means Clustering
The selected algorithm is **K-Means Clustering**, an unsupervised machine learning algorithm used to group data points into $K$ clusters.



### How it works:
1. **Initialization:** Randomly select $K$ centroids.
2. **Assignment:** Each data point is assigned to the nearest centroid based on Euclidean distance:
   $$d(p, q) = \sqrt{\sum_{i=1}^{n} (p_i - q_i)^2}$$
3. **Update:** Centroids are recalculated as the mean of all points in the cluster.
4. **Iteration:** Steps 2 and 3 repeat until the centroids stabilize.

---

## 💻 Implementation Explanations
The implementation in `Assignment2.ipynb` follows these key steps:
1. **Data Preprocessing:** Handling missing values and scaling features using `StandardScaler`.
2. **Elbow Method:** Determining the optimal number of clusters ($K$) by plotting the Within-Cluster Sum of Squares (WCSS).
3. **Model Fitting:** Applying the Scikit-learn `KMeans` class to the processed data.
4. **Visualization:** Plotting the clusters in 2D to observe the grouping of diabetes patients.

---

## 📈 Results Summary
The analysis successfully identified distinct clusters within the diabetes patient data. 
* **Key Finding:** The "Elbow Point" was typically found at $K=3$ or $K=4$, suggesting specific physiological groupings within the dataset.
* **Visualization:** (See screenshots within the [Report](./Report_for_clustering_A2.pdf) for detailed cluster maps and centroid locations).

---

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
