# Customer Segmentation Using K-Means Clustering

## Overview

This project demonstrates the use of the **K-Means Clustering** algorithm for customer segmentation. By grouping customers based on their purchasing behavior and demographics, businesses can develop targeted marketing strategies and improve customer experiences. The implementation is done using a Jupyter Notebook for ease of exploration and visualization.

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
| Feature                 | Description                                   | Type        |
|-------------------------|-----------------------------------------------|-------------|
| **CustomerID**          | Unique identifier for each customer           | Categorical |
| **Age**                 | Age of the customer                          | Numeric     |
| **Annual Income (k$)**  | Annual income of the customer in $1000        | Numeric     |
| **Spending Score (1-100)** | Spending score assigned to the customer   | Numeric     |

### **Target**
Since this is an **unsupervised learning** task, there is no explicit target variable.

---

## Methodology

### **1. Data Exploration**
- Load and inspect the dataset to understand its structure.
- Visualize feature distributions and pairwise relationships to identify potential clusters.

### **2. Data Preprocessing**
- Drop irrelevant columns (e.g., `CustomerID`).
- Normalize features using `StandardScaler` to prepare data for clustering.

### **3. Clustering with K-Means**
- Determine the optimal number of clusters using the **Elbow Method**.
- Apply **K-Means Clustering** with the optimal number of clusters.
- Add cluster labels to the dataset for interpretation.

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
  - `pandas` and `numpy`: For data manipulation.
  - `matplotlib` and `seaborn`: For data visualization.
  - `scikit-learn`: For K-Means Clustering and evaluation.

---

## How to Run

### Step 1: Clone the Repository
Clone the repository to your local machine:
```bash
git clone <repository-url>
cd Customer-Segmentation-Clustering

```

### Step 2: Install Dependencies
Install the required Python libraries using the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

### Step 3: Open the Jupyter Notebook
Launch Jupyter Notebook to interact with the code:
```bash
jupyter notebook "Customer Segmentation.ipynb"
```

### Step 4: Explore the Results
Run the notebook cell by cell to:
- Explore the dataset.
- Perform clustering and visualize the results.
- Evaluate cluster quality and interpret the findings.

---

## Repository Structure

```
project-directory/
│
├── Customer Segmentation.ipynb    # Jupyter Notebook for the tutorial
├── Mall_Customers.csv             # Dataset file
├── requirements.txt               # List of dependencies
├── LICENSE                        # License information
├── README.md                      # Documentation
└── results/                       # Directory for storing visualizations and outputs
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

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Author

This project was created to demonstrate the power of clustering in customer segmentation and its applications in real-world business scenarios.

--- 
