# 📊 Comparative Study of Clustering Algorithms with Preprocessing Techniques

---

## 📌 Objective
The objective of this project is to analyze and compare the performance of different clustering algorithms using various preprocessing techniques and different numbers of clusters. The study evaluates how preprocessing impacts clustering quality.

---

## 📌 Dataset
- **Dataset Used:** Wine Dataset (UCI / sklearn)
- **Number of Samples:** 178
- **Number of Features:** 13
- The dataset contains chemical properties of wines from different cultivars.

---

## 📌 Algorithms Used
- K-Means Clustering
- Hierarchical Clustering (Agglomerative)
- Mean Shift Clustering

---

## 📌 Preprocessing Techniques
The dataset was processed using multiple techniques:
- No preprocessing (Raw data)
- Normalization (StandardScaler)
- Transformation (Power Transformation)
- PCA (Dimensionality Reduction)
- Transform + Normalize (T + N)
- Transform + Normalize + PCA (T + N + PCA)

---

## 📌 Evaluation Metrics
The clustering performance was evaluated using:

- **Silhouette Score** → Higher is better  
- **Calinski-Harabasz Index** → Higher is better  
- **Davies-Bouldin Score** → Lower is better  

---

## 📊 Results

The results were recorded for different clustering algorithms and preprocessing combinations. The detailed results are available in:

📁 `clustering_results.csv`

---

## 📈 Graphical Analysis

### 🔹 Silhouette Score Comparison
![Silhouette Score](graph/ss.png)

---

### 🔹 Calinski-Harabasz Score
![Calinski-Harabasz](graph/ch.png)

---

### 🔹 Davies-Bouldin Score
![Davies-Bouldin](graph/db.png)

---

### 🔹 K-Means Clustering Visualization (PCA 2D)
![KMeans PCA](graph/image.png)

---

## 🔍 Key Observations

- Normalization significantly improved the performance of distance-based algorithms like K-Means.
- PCA helped in reducing dimensionality and improved cluster separation visually.
- K-Means performed consistently well across most preprocessing techniques.
- Hierarchical clustering showed stable results but was slightly less effective for higher cluster values.
- Mean Shift did not perform consistently across all preprocessing techniques.
- The best clustering performance was generally observed when **K = 3**, aligning with the dataset structure.

---

## 📌 Conclusion

- Preprocessing plays a crucial role in improving clustering performance.
- K-Means combined with normalization or PCA produced the most reliable results.
- PCA enhances visualization but may lead to slight information loss.
- Choosing the right number of clusters and preprocessing technique is essential for optimal clustering.

---

## 🚀 Future Improvements

- Experiment with more clustering algorithms (DBSCAN, Gaussian Mixture Models)
- Use larger and more complex datasets
- Hyperparameter tuning for better optimization
