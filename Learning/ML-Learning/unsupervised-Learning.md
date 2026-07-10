# 🤖 Unsupervised Learning

> Unsupervised Learning is a type of Machine Learning in which the model learns from **unlabeled data** and automatically discovers hidden patterns and relationships.

---

## 📌 Introduction

Unlike supervised learning, there are no predefined output labels in unsupervised learning. The algorithm analyzes the dataset and groups similar data points together.

---

## ⚙️ How Unsupervised Learning Works

1. 📂 Collect the dataset.
2. 📊 Provide unlabeled data to the algorithm.
3. 🔍 Analyze the data and identify patterns.
4. 🧩 Group similar data points.
5. 📈 Use the discovered patterns for analysis and decision-making.

---

## 🖼️ Unsupervised Learning Diagram

<p align="center">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20251210102132756957/unsupervised_learning.webp" width="650">
</p>

---

# 📚 Types of Unsupervised Learning

## 1️⃣ Clustering

Clustering is the process of grouping similar data points into different clusters.

### 🎯 Applications

* Customer segmentation
* Recommendation systems
* Image classification
* Document categorization

### 🛠️ Popular Algorithms

* K-Means Clustering
* Hierarchical Clustering
* DBSCAN

---

### 🖼️ Clustering Diagram

<p align="center">
    <img src="https://serokell.io/files/a7/a74cj5c.Clustering_Algorithms_pic2.jpg" alt="Clustering Diagram" width="500">
</p>

---

## 2️⃣ Association

Association identifies relationships between different items in a dataset.

### 🎯 Applications

* Market basket analysis
* Product recommendations
* Customer behavior analysis

### 🛠️ Popular Algorithms

* Apriori Algorithm
* ECLAT Algorithm
* FP-Growth Algorithm

---

## 3️⃣ Dimensionality Reduction

Dimensionality reduction reduces the number of features while preserving important information.

### 🎯 Applications

* Data visualization
* Noise reduction
* Faster model training

### 🛠️ Popular Algorithms

* PCA (Principal Component Analysis)
* t-SNE

---

### 🖼️ PCA Diagram

<p align="center">
    <img src="https://www.scaler.com/topics/images/concept-of-pca.webp" alt="PCA Diagram" width="500">
</p>

---

# ✅ Advantages

* ✔️ No labeled data is required.
* ✔️ Helps discover hidden patterns.
* ✔️ Works well with large datasets.
* ✔️ Reduces manual effort.

---

# ❌ Disadvantages

* ❌ Results can be difficult to interpret.
* ❌ Accuracy is hard to measure.
* ❌ Choosing the right algorithm can be challenging.

---

# 🌍 Real-World Applications

* 💳 Fraud detection
* 🎬 Recommendation systems
* 👥 Customer segmentation
* 🌐 Social network analysis
* 🛒 Market basket analysis

---

# 🚀 Conclusion

Unsupervised Learning helps machines discover hidden patterns in unlabeled data. It is widely used in clustering, recommendation systems, data analysis, and feature reduction.

⭐ It plays an important role in solving real-world problems where labeled data is unavailable.

# 🎯 K-Means Clustering

> K-Means Clustering is one of the most popular **unsupervised machine learning algorithms** used to group similar data points into different clusters.

---

## 📌 Introduction

K-Means Clustering organizes data into **K clusters** based on similarity.

* **K** ➝ Number of clusters.
* **Means** ➝ Average value (centroid) of each cluster.

The algorithm groups similar data points together and separates dissimilar points into different clusters.

---

## ⚙️ Working of K-Means Clustering

The K-Means algorithm follows these steps:

1. 🎯 Choose the number of clusters (**K**).
2. 📍 Randomly select **K centroids**.
3. 🔍 Assign each data point to the nearest centroid.
4. 📊 Calculate the new centroid of each cluster.
5. 🔁 Repeat the process until the centroids stop changing.

---

## 🖼️ K-Means Diagram

<p align="center">
    <img src="https://images.squarespace-cdn.com/content/v1/5acbdd3a25bf024c12f4c8b4/1608407348392-22767PJ7RQ85BD5RLSLZ/k-means-clustering.png" alt="K-Means Clustering Diagram" width="650">
</p>

---

## 💡 Example

Suppose an online shopping website has customer information such as:

* 👤 Age
* 💰 Salary
* 🛒 Purchase History

K-Means can divide customers into different groups based on similar buying behavior.

---

## 🎯 Applications

* 👥 Customer Segmentation
* 🎬 Recommendation Systems
* 🖼️ Image Compression
* 📄 Document Classification
* 📈 Market Analysis

---

## ✅ Advantages

* ✔️ Easy to understand and implement.
* ✔️ Fast and efficient for large datasets.
* ✔️ Works well with clearly separated clusters.

---

## ❌ Disadvantages

* ❌ Choosing the correct value of **K** is difficult.
* ❌ Sensitive to outliers.
* ❌ Does not perform well with irregularly shaped clusters.

---

## 🚀 Popular Uses

* 📊 Business Analytics
* ⛏️ Data Mining
* 🔎 Pattern Recognition
* 🖼️ Image Processing

---

## 🏁 Conclusion

K-Means Clustering is a simple yet powerful algorithm that groups similar data points into clusters. It is widely used in machine learning, data analysis, recommendation systems, and business analytics.

⭐ It is one of the most commonly used clustering techniques in real-world applications.


# 🌳 Hierarchical Clustering

> Hierarchical Clustering is an **unsupervised machine learning algorithm** that groups similar data points into clusters and creates a hierarchy of clusters.

---

## 📌 What is Hierarchical Clustering?

Hierarchical Clustering builds a tree-like structure called a **Dendrogram**, which shows how clusters are formed.

Unlike K-Means, you do not need to specify the number of clusters beforehand.

---

## 🛠️ Types of Hierarchical Clustering

### 🔹 Agglomerative Clustering (Bottom-Up)

* Initially, each data point is treated as a separate cluster.
* The closest clusters are merged step by step.
* The process continues until all points belong to a single cluster.

### 🔹 Divisive Clustering (Top-Down)

* Initially, all data points belong to one cluster.
* The cluster is repeatedly divided into smaller clusters.
* The process continues until every data point becomes its own cluster.

---

## ⚙️ Working of Hierarchical Clustering

1. Consider each data point as a separate cluster.
2. Calculate the distance between all clusters.
3. Merge the two closest clusters.
4. Update the distance matrix.
5. Repeat the process until only one cluster remains.

---

## 🌲 Dendrogram Diagram

<p align="center">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20250526124835660066/What-is-a-Dendrogram_.webp" alt="Dendrogram Diagram" width="650">
</p>

---

## 📏 Distance Measurement Methods

* Euclidean Distance
* Manhattan Distance
* Minkowski Distance
* Cosine Similarity

---

## 🔗 Linkage Methods

| Method           | Description                                  |
| ---------------- | -------------------------------------------- |
| Single Linkage   | Uses the shortest distance between clusters. |
| Complete Linkage | Uses the maximum distance between clusters.  |
| Average Linkage  | Uses the average distance between clusters.  |
| Ward Linkage     | Minimizes the variance within clusters.      |

---

## 🎯 Applications

* Customer segmentation
* Image processing
* Document clustering
* Biological data analysis
* Recommendation systems

---

## ✅ Advantages

* No need to choose the number of clusters in advance.
* Easy to visualize using a dendrogram.
* Works well with small datasets.

---

## ❌ Disadvantages

* Computationally expensive for large datasets.
* Sensitive to noise and outliers.
* Difficult to undo cluster merges.

---

## 🚀 Conclusion

Hierarchical Clustering is a powerful unsupervised learning technique that organizes data into a tree-like structure. It is useful for discovering hidden patterns and relationships between data points.

# 🔍 DBSCAN Clustering

## 📌 Introduction

DBSCAN (**Density-Based Spatial Clustering of Applications with Noise**) is an unsupervised machine learning algorithm that groups nearby data points based on density.

Unlike K-Means, DBSCAN does not require the number of clusters in advance and can identify outliers (noise).

---

## ⚙️ How DBSCAN Works

1. Select two parameters:

   * **Epsilon (ε):** Maximum distance between points.
   * **MinPts:** Minimum number of points required to form a cluster.

2. Find neighboring points within the ε distance.

3. Create clusters from dense regions.

4. Mark isolated points as **noise**.

---

## 📊 Types of Points

* **Core Point**
* **Border Point**
* **Noise Point**

---

## 🖼️ Diagram

<p align="center">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20250912171108762993/frame_3073.webp" alt="DBSCAN Clustering Diagram" width="600">
</p>

---

## 🎯 Applications

* Customer segmentation
* Fraud detection
* Image processing
* Social network analysis

---

## ✅ Advantages

* No need to specify the number of clusters.
* Detects outliers automatically.
* Works well with irregular-shaped clusters.

---

## ❌ Disadvantages

* Sensitive to parameter selection.
* Not suitable for varying-density datasets.

---

## 🚀 Conclusion

DBSCAN is a density-based clustering algorithm that groups similar data points and automatically detects noise in the dataset.


# 🛒 Apriori Algorithm

## 📌 Introduction

Apriori is an **unsupervised machine learning algorithm** used for **association rule learning**. It helps discover relationships between items in large datasets.

It is mainly used in **Market Basket Analysis**, where stores analyze which products customers frequently buy together.

---

## 💡 Example

Suppose customers often buy:

* 🥛 Milk
* 🍞 Bread
* 🧈 Butter

The Apriori algorithm can find patterns such as:

> Customers who buy **Milk** are also likely to buy **Bread** and **Butter**.

---

## ⚙️ How Apriori Works

1. Find frequently purchased items.
2. Generate item combinations.
3. Calculate support and confidence.
4. Create association rules.

---

## 📊 Important Terms

| Term           | Meaning                                           |
| :------------- | :------------------------------------------------ |
| **Support**    | How often an item appears in the dataset.         |
| **Confidence** | Probability that one item is bought with another. |
| **Lift**       | Measures the strength of the association rule.    |

---

## 🖼️ Diagram

<p align="center">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20250917144620984191/apriori_algorithm_1.webp" alt="Apriori Algorithm Diagram" width="650">
</p>

---

## 🎯 Applications

* Market basket analysis
* Product recommendations
* Customer behavior analysis
* Sales and marketing

---

## ✅ Advantages

* Easy to understand and implement.
* Finds hidden relationships in data.
* Useful for recommendation systems.

---

## ❌ Disadvantages

* Slow for very large datasets.
* Requires high computational power.
* Generates many candidate itemsets.

---

## 🚀 Conclusion

Apriori is a popular association-rule algorithm that helps discover patterns and relationships between items in large datasets. It is widely used in recommendation systems and market analysis.

# 🌳 FP-Growth Algorithm

## 📌 Introduction

FP-Growth (Frequent Pattern Growth) is an unsupervised machine learning algorithm used to find frequent itemsets in large datasets.

It is faster than Apriori because it does not generate candidate itemsets repeatedly.

---

## ⚙️ Working of FP-Growth

1. Scan the dataset.
2. Find frequent items.
3. Build an FP-Tree.
4. Extract frequent patterns from the tree.

---

## 🎯 Applications

- Market basket analysis
- Recommendation systems
- Customer behavior analysis

---

## 🖼️ Diagram

<p align="center">
    <img src="https://media.geeksforgeeks.org/wp-content/uploads/20251115111735684932/_frequent_pattern_growth_algorithm.webp" alt="FP-Growth Diagram" width="650">
</p>

---

# 🔗 ECLAT Algorithm

## 📌 Introduction

ECLAT (Equivalence Class Clustering and Bottom-up Lattice Traversal) is an association rule learning algorithm used to find frequent itemsets.

It uses a vertical database format, making the algorithm faster.

---

## ⚙️ Working of ECLAT

1. Convert the dataset into a vertical format.
2. Find common transaction IDs.
3. Generate frequent itemsets.

---

## 🎯 Applications

- Product recommendation
- Market basket analysis

## ⚡ FP-Growth vs ECLAT

| Feature | FP-Growth | ECLAT |
|----------|----------|--------|
| Data Structure | FP-Tree | Vertical Database |
| Speed | Faster | Fast |
| Memory Usage | Less | More |
| Main Use | Pattern Mining | Association Rules |

