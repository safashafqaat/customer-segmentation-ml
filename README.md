# 🛒 Customer Segmentation using K-Means & DBSCAN

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)
![Seaborn](https://img.shields.io/badge/Seaborn-EDA-red)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)

---

##  Project Overview
This project applies **customer segmentation** on the [Mall Customers Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).  
The goal is to group customers based on **Annual Income** and **Spending Score**, helping businesses design targeted marketing campaigns.

---

##  Objectives
- Perform **Exploratory Data Analysis (EDA)** to understand customer distribution.
- Apply **feature scaling** using StandardScaler.
- Use **K-Means Clustering** and determine optimal number of clusters with **Elbow Method** & **Silhouette Score**.
- Visualize clusters in 2D with centroids.
- Compare results with **DBSCAN (Density-Based Spatial Clustering)**.
- Analyze **average spending & income per cluster** for business insights.

---

##  Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Workflow
1. **Data Loading & Cleaning**
   - Load Mall Customers dataset
   - Inspect data types & missing values
   - Summary statistics

2. **Exploratory Data Analysis**
   - Boxplots for numerical features
   - Pie chart for gender distribution

3. **Preprocessing**
   - Select features: `Annual Income (k$)` and `Spending Score (1-100)`
   - Apply `StandardScaler` for normalization

4. **Clustering**
   - K-Means with Elbow & Silhouette method to find optimal clusters
   - Final KMeans model with **k=5**
   - Scatter plot of clusters with **fixed colors**:
     - 🟢 Green → Budget Shoppers  
     - 🔴 Red → Premium Customers  
     - 🟤 Brown → Potential Loyalists  
     - ⚪ Grey → Average Customers  
     - 🟠 Orange → Young Trendsetters  
   - Centroids shown as **black stars (★)**

5. **DBSCAN**
   - Alternative clustering approach
   - Detects dense clusters and outliers

6. **Cluster Analysis**
   - Average income & spending per cluster
   - Business interpretation of clusters

---

## Results
- Identified **5 distinct customer segments** using KMeans:
  - 🟢 **Budget Shoppers** – Low income, low spending  
  - 🔴 **Premium Customers** – High income, high spending  
  - 🟤 **Potential Loyalists** – High income, low spending  
  - ⚪ **Average Customers** – Medium income & spending  
  - 🟠 **Young Trendsetters** – Medium income, high spending  

---

##  How to Run
Clone the repository:
```bash
git clone https://github.com/safashafqaat/customer-segmentation-ml.git
cd customer-segmentation-ml
