# Customer Segmentation using K-Means Clustering

This project performs customer segmentation on the Mall Customers dataset using K-Means clustering. It helps understand customer behavior by grouping similar customers together based on features like Annual Income and Spending Score.

## 📌 Objective

The aim is to segment customers into distinct clusters based on their income and spending patterns. This kind of segmentation can be highly useful for targeted marketing strategies.

---

## 🗂 Dataset

- **Source**: `Mall_Customers.csv`
- **Features used**:
  - `Annual Income (k$)`
  - `Spending Score (1-100)`
  
These two features are selected for 2D visualization of clusters.

---

## ✅ Steps Performed

### 1. Data Loading and Preprocessing
- Loaded the dataset and removed unnecessary columns (like `CustomerID`).
- Encoded categorical features and checked for missing values.
- Standardized the selected numerical features for better clustering performance.

### 2. Optimal Cluster Selection - Elbow Method
- Used the Elbow Method to find the optimal number of clusters (`k`) by plotting Within-Cluster Sum of Squares (WCSS) against different values of `k`.

### 3. K-Means Clustering
- Applied K-Means clustering on the scaled features.
- Selected `k = 5` based on the elbow plot.
- Predicted cluster labels for each data point.

### 4. Visualization
- Visualized the 5 clusters in a 2D scatter plot using different colors.
- Cluster centroids were highlighted in yellow.

### 5. Evaluation - Silhouette Score
- Calculated the **Silhouette Score** to evaluate clustering performance.
- A higher score (close to 1) indicates well-defined and meaningful clusters.

---

## 📊 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 📌 Conclusion

- The model successfully segmented customers into 5 groups with distinct spending behaviors.
- Visualization showed clear separation between clusters.
- The Silhouette Score provided a good quantitative measure of clustering quality.

---

## 🚀 Future Improvements

- Use all features (including Age and Gender) and apply **PCA** for dimensionality reduction.
- Try other clustering algorithms like **DBSCAN** or **Hierarchical Clustering** for comparison.

---

## 💡 Use Case

Businesses can use this segmentation to:
- Customize marketing campaigns.
- Offer personalized deals.
- Improve customer retention strategies.

