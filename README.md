# 🧱 Concrete Mixture Clustering using Machine Learning

> A clustering project to group concrete compositions by their mix components and compressive strengths using K-Means and Hierarchical clustering techniques.

---

## 📟 Abstract

This project uses a dataset of concrete mixtures to group samples based on their compositional components using unsupervised clustering methods. The dataset includes 1,030 samples with 11 features such as cement, water, age, and other ingredients. The goal is to identify natural groupings of concrete types to support construction material optimization and smarter building strategies. Two clustering algorithms, K-Means and Agglomerative Hierarchical Clustering, were applied and compared.

---

## 📘 Introduction

Concrete compressive strength is influenced by multiple mix components. This dataset includes features such as cement, water, fly ash, superplasticizer, and more. Understanding the natural groupings within the data helps in optimizing mixtures for different construction needs.

### Dataset Reference:

[https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength](https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength)

---

## 🌟 Goal

* Cluster concrete mixtures based on their features using unsupervised learning.
* Compare K-Means and Hierarchical clustering.
* Evaluate clustering quality using silhouette scores.
* Support businesses in optimizing concrete mix recipes for cost, strength, and environmental impact.

---

## 💡 Key Novelty

* Application of clustering for concrete quality analysis.
* Evaluation using both elbow method and silhouette score.
* Ethical focus on proper representation and safe grouping of data.
* Real-world application in construction and material sciences.

---

## ⚙️ Methodology

### 1. Data Preprocessing & EDA

* Dataset loaded and explored using `pandas`, `head()`, `info()`, and `describe()`.
* Verified that no missing values existed.
* Removed categorical columns (fly ash and concrete type) unsuitable for clustering.
* Standardized numerical features using `StandardScaler` to align scales.

### 2. Clustering Algorithms

#### 🔹 K-Means Clustering

* Used elbow method and silhouette analysis to determine optimal clusters: **k = 5**
* Reduced dimensions using PCA for 2D visualization
* Visualized cluster centers and sample distributions
* Silhouette score: **0.247** (moderate clustering quality)

#### 🔹 Agglomerative Hierarchical Clustering

* Used dendrogram to determine optimal clusters: **6 clusters**
* Applied `AgglomerativeClustering` from `sklearn`
* Visualized results in 2D using PCA
* Silhouette score: **0.2417** (comparable to K-Means)

---

## 📊 Results

| Algorithm                | Optimal Clusters | Silhouette Score | Comments                               |
| ------------------------ | ---------------- | ---------------- | -------------------------------------- |
| K-Means                  | 5                | 0.247            | Moderate separation                    |
| Agglomerative Clustering | 6                | 0.2417           | Similar result, slightly less cohesive |

* The data is compact and exhibits overlapping samples
* Both methods show acceptable but not perfect grouping

---

## 🏗️ Business Applications

### Construction Use Cases

* Identify recipes for **high-performance vs. standard concrete**
* Use cluster profiles as templates for specific construction needs:

  * Bridges, towers (high strength)
  * Pavements (low cost)

### Recipe Optimization

* Focus R\&D efforts on clusters with high strength and low cement (more eco-friendly)
* Identify and phase out underperforming mixtures

### Actionable Recommendations

* Categorize products as "economy", "standard", and "high-performance"
* Educate clients about best-fit mixes for specific applications
* Automate cluster-based concrete design in CAD/building systems
* Promote sustainability by focusing on efficient compositions

---

## 🧠 Conclusion

Both K-Means and Agglomerative Clustering revealed moderately distinct clusters of concrete mixtures. These groupings can help businesses streamline material usage, optimize cost-performance balance, and offer targeted solutions for different construction applications. While silhouette scores suggest room for improvement, the clustering approach offers practical and scalable benefits for construction optimization.


---

## 📜 License

This project is released under the MIT License.

---

## 🙋 Author

**\[Syed Ali Murtaza]**
GitHub: [alishah-00001](https://github.com/alishah-00001)
