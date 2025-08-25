# RFM_and_Churn_Prediction
# Customer Segmentation & Churn Prediction using RFM Analysis and Machine Learning

## Project Overview
This project leverages **RFM Analysis** for customer segmentation and applies **Machine Learning models** to predict churn for an online retail company based in the UK. The goal is to help businesses identify high-value customers, understand purchasing patterns, and proactively manage churn risk through data-driven insights.

---

## Dataset
- **Source:** Online retail dataset of a UK-based company (transaction-level data).  
- **Key Fields:**  
  `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA) & Visualization
- Data cleaning (handling missing values, duplicates, and cancellations).
- Descriptive statistics and purchase behavior trends.
- Visualizations:
  - Revenue and Average Order Value per country
  - Revenue Heatmap: Hour vs Day of the week
  - Product lifecycle analysis

---

### 2. RFM Analysis (Customer Segmentation)
- **Recency (R):** Days since last purchase.  
- **Frequency (F):** Number of purchases.  
- **Monetary (M):** Total spending per customer.  
- Standardized RFM scores for clustering.  
- **K-Means Clustering**:
  - Optimal `k` selected using Elbow Method & Silhouette Score.
  - Customer groups identified:  Potential Loyalists, Lost Customers, Champions (VIP), Loyal Big Spenders

---

### 3. Customer Churn Prediction (Classification)
- **Churn Label Creation:**  
  Defined churn based on inactivity in the final observation period.
- **Feature Engineering:**  
  - Visit frequency, quantity purchased, product diversity, and basket size in each of the last 4 months.
- **Models Used:**
  - Logistic Regression  
  - Random Forest  
  - XGBoost (final model after hyperparameter tuning with **Optuna**)
- **Evaluation Metrics:**  
  Accuracy, Precision, Recall, F1-Score, ROC-AUC.

---

## Tech Stack
- **Languages & Libraries:** Python (Pandas, NumPy, Scikit-learn, XGBoost, Optuna, Matplotlib, Seaborn)
- **Techniques:** RFM Analysis, K-Means Clustering, Feature Engineering, Hyperparameter Optimization, Classification Modeling.

---

## Key Outcomes
- Identified distinct customer segments for targeted marketing.
- Built a churn prediction model with optimized parameters to flag at-risk customers.
- Provided actionable insights to improve **customer retention** and **lifetime value (CLV)**.

---

