# **Mall Customer Segmentation**

## **Overview**
This project focuses on **customer segmentation** to help businesses tailor their marketing strategies effectively. By analyzing customer demographics and spending behavior, the goal is to identify distinct customer groups and provide insights that drive **targeted marketing efforts**.

## **Dataset**
The dataset consists of **200 customers** with the following features:
- **CustomerID** – Unique identifier  
- **Gender** – Male (1), Female (0)  
- **Age** – Customer’s age  
- **Annual Income (k$)** – Customer's annual income in thousands of dollars  
- **Spending Score (1-100)** – Score representing spending behavior and loyalty  

## **Data Preprocessing**
✔ Checked for **missing values** → None found  
✔ **Label encoding** applied to categorical variables  
✔ **Feature normalization** for fair clustering  

## **Methodology**
The project employs **two clustering techniques**:  
1. **K-Means Clustering** (Implemented from scratch)  
2. **Hierarchical Clustering** (Using `sklearn`)  

### **1️⃣ K-Means Clustering**
- **Process:**  
  - Random initialization of centroids  
  - Iterative updates to minimize intra-cluster distances  
  - Stopping condition: Centroids remain stable  
- **Performance Metric:**  
  - **Silhouette Score** → **0.458** (indicating well-defined clusters)  

### **2️⃣ Hierarchical Clustering**
- **Process:**  
  - Uses an **agglomerative** approach (bottom-up clustering)  
  - Forms clusters by minimizing variance within each group  
  - **Visualized using a dendrogram**  
- **Performance Metric:**  
  - **Silhouette Score** → **0.446** (slightly lower than K-Means)  

## **Cluster Analysis & Interpretation**
Three clusters were identified with the following characteristics:

### **🔹 Cluster 0 (Budget-Conscious Customers)**
- **Middle-aged individuals**  
- **Slightly below-average income**  
- **Moderate spending scores**  
- **Ideal for promotions and discounts**  

### **🔹 Cluster 1 (Cautious Spenders)**
- **Older individuals**  
- **Average income, low spending score**  
- **Focuses on essential & practical purchases**  

### **🔹 Cluster 2 (High-Spending Customers – 💰 Target Group)**
- **Younger individuals**  
- **Above-average income**  
- **Highest spending scores**  
- **Prime candidates for premium products & lifestyle promotions**  

## **Visualization & Insights**
### **📌 K-Means Clustering Visualization**
- **Clusters are well-separated** with minimal overlap.  
- **Each cluster is distinctly colored**, representing customer segmentation effectively.  

### **📌 Hierarchical Clustering Dendrogram**
- **Two main clusters** with distinct separations.  
- **Further sub-clusters** indicate smaller customer groups within broader categories.  

## **Model Evaluation**
- **Silhouette Scores**:  
  - **K-Means**: **0.458** (better clustering)  
  - **Hierarchical**: **0.446**  
- **K-Means outperforms Hierarchical Clustering**, producing better-defined customer groups.  

## **🎯 Target Customer Recommendations**
- **Focus on Cluster 2 (Affluent & High-Spending Customers)**  
- **Marketing Strategies:**  
  - Personalized offers  
  - Exclusive discounts  
  - Loyalty programs  
  - High-value product promotions  

## **Conclusion**
This project successfully segments mall customers based on their demographic and financial behaviors.  
✔ **K-Means clustering provided better-defined clusters** compared to Hierarchical clustering.  
✔ **Businesses can use these insights to enhance engagement and increase sales** by targeting specific customer groups.  

