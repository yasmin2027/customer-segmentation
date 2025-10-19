# Mall Customers Clustering using K-Means

## Project Overview
This project applies **K-Means Clustering**, an unsupervised machine learning algorithm, to segment mall customers into distinct groups based on their **Annual Income** and **Spending Score**.  
The goal is to help businesses understand different customer segments for better marketing strategies.

---

## Objectives
- Analyze customer data from the Mall Customers dataset.  
- Use the **Elbow Method** to determine the optimal number of clusters.  
- Apply **K-Means Clustering** to segment customers.  
- Visualize the clusters and centroids clearly.  

---

## Dataset Information
**Dataset:** `Mall_Customers.csv`

| Feature | Description |
|----------|-------------|
| `CustomerID` | Unique ID for each customer |
| `Gender` | Male or Female |
| `Age` | Age of the customer |
| `Annual Income (k$)` | Annual income in thousands |
| `Spending Score (1-100)` | Score assigned by the mall based on spending patterns |

---

## Libraries Used
- **Pandas** → For data handling  
- **Matplotlib** → For visualizing clusters  
- **Scikit-learn (sklearn)** → For K-Means Clustering  

---

## Steps in the Project

1. **Load Dataset**  
   Imported data using Pandas and selected relevant features (`Annual Income (k$)` and `Spending Score (1-100)`).

2. **Determine Optimal Clusters (Elbow Method)**  
   - Calculated Within-Cluster Sum of Squares (WCSS) for cluster numbers 1 to 10.  
   - Visualized the elbow curve to choose the best number of clusters (5).  

3. **Apply K-Means Clustering**  
   - Created a model with 5 clusters using `KMeans(n_clusters=5, init='k-means++')`.  
   - Added a new column `Cluster` to the dataset for assigned cluster labels.  

4. **Visualize Clusters**  
   - Plotted customer groups by income and spending score.  
   - Highlighted centroids with black “X” markers.

---

## Results
The algorithm successfully divided the customers into **five distinct clusters**, such as:
- **High Income, High Spending**  
- **High Income, Low Spending**  
- **Average Income, Average Spending**  
- **Low Income, High Spending**  
- **Low Income, Low Spending**

These insights can be used for **targeted marketing** and **customer relationship management**.

---

## Future Improvements
- Include **Age** and **Gender** for multi-dimensional clustering.  
- Use **DBSCAN** or **Hierarchical Clustering** for comparison.  
- Apply **Principal Component Analysis (PCA)** for visualization in higher dimensions.




