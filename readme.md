# **Clustering Analysis on UCI Dataset**

## **Project Overview**

This project performs a comparative performance analysis of different clustering algorithms (**K-Means**, **Hierarchical Clustering**, and **Mean-Shift Clustering**) using various preprocessing techniques. The Iris dataset from the UCI repository has been used for clustering and evaluation.

The preprocessing techniques applied are:

1. **No Data Processing**
2. **Normalization**
3. **PCA (Principal Component Analysis)**
4. **Combination Techniques (T+N, T+N+PCA)**

The performance of clustering algorithms is evaluated using the following metrics:

- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Score**

---

## **Dataset**

**Dataset Name**: Iris Dataset  
**Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data)  
**Description**:  
The dataset contains 4 numerical features:

- `sepal_length`, `sepal_width`, `petal_length`, `petal_width`  
  The target class is removed for unsupervised clustering.

---

## **Steps in the Project**

1. **Import Libraries**  
   Libraries: `pandas`, `numpy`, `sklearn`, `matplotlib`, `seaborn`

2. **Load Dataset**

   - The Iris dataset is loaded.
   - Target labels are dropped since clustering is unsupervised.

3. **Preprocessing Techniques**

   - **No Data Processing**
   - **Normalization** (Using `MinMaxScaler`)
   - **PCA** (Reduced dimensions to 2 components using `PCA`)
   - Combined Techniques (`Normalization + PCA`)

4. **Clustering Algorithms**

   - **K-Means Clustering**
   - **Hierarchical Clustering**
   - **Mean-Shift Clustering**

5. **Performance Evaluation**  
   Metrics used:

   - **Silhouette Score** (Higher is better)
   - **Calinski-Harabasz Index** (Higher is better)
   - **Davies-Bouldin Score** (Lower is better)

6. **Results Visualization**

   - Scatter plots of clusters (using PCA-reduced data).

7. **Results Comparison**  
   A detailed performance comparison table is created for all algorithms and preprocessing techniques.

---

## **Code Structure**

The project consists of the following steps in the Colab notebook:

```bash
1. Load Libraries
2. Load and Prepare Dataset
3. Apply Preprocessing Techniques:
   - No Processing
   - Normalization
   - PCA
   - Combined Techniques
4. Define Clustering and Evaluation Functions
5. Run Clustering Algorithms:
   - K-Means
   - Hierarchical
   - Mean-Shift
6. Compare Performance Metrics
7. Visualize Clusters
8. Results Summary
```
