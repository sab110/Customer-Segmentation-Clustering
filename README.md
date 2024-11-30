# Customer Segmentation Using K-Means Clustering

## Overview

This project demonstrates the use of the **K-Means Clustering** algorithm for customer segmentation. By grouping customers based on their purchasing behavior and demographics, businesses can develop targeted marketing strategies and improve customer experiences.

---

## Objectives

1. Perform customer segmentation using **K-Means Clustering**.
2. Explore and preprocess the dataset to prepare it for clustering.
3. Determine the optimal number of clusters using the **Elbow Method**.
4. Visualize the clusters to interpret customer groupings.
5. Evaluate the quality of clustering using the **Silhouette Score**.

---

## Dataset

### **Source**
The dataset is available on [Kaggle](https://www.kaggle.com/datasets/sonalisingh1411/mallcustomersdataset?resource=download).

### **Features**
| Feature              | Description                                   | Type        |
|----------------------|-----------------------------------------------|-------------|
| **CustomerID**       | Unique identifier for each customer           | Categorical |
| **Age**              | Age of the customer                          | Numeric     |
| **Annual Income (k$)** | Annual income of the customer in $1000       | Numeric     |
| **Spending Score (1-100)** | Spending score assigned to the customer | Numeric     |

### **Target**
Since this is an **unsupervised learning** task, there is no explicit target variable.

---

## Methodology

### **1. Data Exploration**
- Explore the dataset to understand feature distributions and relationships.
- Visualize pairwise relationships to identify potential clusters.

### **2. Data Preprocessing**
- Drop irrelevant columns (e.g., `CustomerID`).
- Normalize features using `StandardScaler` to prepare data for clustering.

### **3. Clustering with K-Means**
- Determine the optimal number of clusters using the **Elbow Method**.
- Apply **K-Means Clustering** with the optimal number of clusters.
- Add cluster labels to the original dataset for interpretation.

### **4. Visualizing Clusters**
- Use 2D scatter plots to visualize clusters (e.g., Spending Score vs. Annual Income).
- Optionally, extend to 3D visualizations for deeper insights.

### **5. Evaluate Clustering**
- Use the **Silhouette Score** to assess cluster quality (cohesion and separation).

---

## Results and Insights

### **Key Findings**
1. **Segmentation**: Customers were grouped into **5 distinct clusters**, each representing a unique purchasing pattern.
2. **Optimal Clusters**: The **Elbow Method** identified 5 as the ideal number of clusters.
3. **Cluster Evaluation**: The **Silhouette Score** confirmed the effectiveness of the clustering, indicating well-separated and cohesive clusters.

### **Applications**
1. **Targeted Marketing**: Focus marketing campaigns on high-spending clusters.
2. **Customer Retention**: Develop strategies to retain customers in at-risk clusters.
3. **Resource Allocation**: Allocate resources based on cluster-specific needs.

---

## Tools and Libraries

- **Programming Language**: Python
- **Libraries**:
  - `pandas` and `numpy` for data manipulation.
  - `matplotlib` and `seaborn` for data visualization.
  - `sklearn` for K-Means Clustering and evaluation.

---

## How to Run

1. Clone the repository and navigate to the project directory:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script or notebook:
   ```bash
   python customer_segmentation.py
   ```

---

## Future Work

1. **Advanced Clustering**:
   - Experiment with **DBSCAN** or **Hierarchical Clustering** for more nuanced groupings.
2. **Feature Engineering**:
   - Create new features based on domain knowledge to improve clustering results.
3. **Business Integration**:
   - Use domain expertise to interpret clusters and align findings with business objectives.

---

## Author

This project was created to demonstrate the power of clustering in customer segmentation and its applications in real-world business scenarios.
```
