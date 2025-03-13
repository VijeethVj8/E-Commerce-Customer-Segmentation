# 📊 E-Commerce Customer Segmentation

This project focuses on **customer segmentation** for an online retail dataset using **K-Means clustering**. The goal is to **enhance marketing strategies** by identifying different customer groups based on their purchasing behavior.

## 📌 **Project Overview**
This dataset contains transactions from a **UK-based online retailer** (2010-2011). The objective is to **segment customers** based on:
- **Recency**: How recently a customer made a purchase.
- **Frequency**: How often they purchase.
- **Monetary Value**: How much they spend.

## 🛠️ **Technologies Used**
- Python 🐍
- Pandas, NumPy (Data Processing)
- Matplotlib, Seaborn (Visualization)
- Scikit-Learn (Clustering with K-Means)

## 📂 **Dataset**
The dataset is sourced from the **UCI Machine Learning Repository**. It consists of:
- `InvoiceNo`: Transaction ID
- `StockCode`: Product ID
- `Description`: Product details
- `Quantity`: Number of units purchased
- `InvoiceDate`: Date & time of transaction
- `UnitPrice`: Price per unit
- `CustomerID`: Unique customer identifier
- `Country`: Customer's country

## 📊 **Steps Completed**
### 🔹 **1. Data Preprocessing**
- Handled **missing values** (`CustomerID`, `Description`)
- Converted `InvoiceDate` to **datetime format**
- Removed **negative/zero quantity transactions**
- Dropped **duplicates**

### 🔹 **2. Feature Engineering**
Created three key customer features:
- `Recency`: Days since last purchase.
- `Frequency`: Number of unique purchases.
- `MonetaryValue`: Total amount spent.

### 🔹 **3. Exploratory Data Analysis (EDA)**
- Analyzed distributions of **Recency, Frequency, and Monetary Value**.
- Identified **outliers** and spending patterns.

### 🔹 **4. Customer Segmentation with K-Means**
- Applied **MinMaxScaler** to normalize data.
- Used **Elbow Method** to determine **optimal K**.
- Applied **K-Means clustering** to segment customers.

### 🔹 **5. Cluster Analysis & Business Insights**
- **Cluster 0**: Moderate buyers (encourage repeat purchases).
- **Cluster 1**: VIP customers (retain loyalty).
- **Cluster 2**: Churned customers (reactivate engagement).

## 📈 **Key Findings**
- Most customers **shop infrequently** and spend less.
- A **small VIP segment** contributes significantly to revenue.
- **Inactive customers** need re-engagement strategies.

## 🎯 **Future Work**
- Implement a **recommendation system** for product suggestions.
- Integrate segmentation into **real-world CRM applications**.
- Experiment with **other clustering techniques (DBSCAN, Hierarchical Clustering)**.

## 🚀 **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/ecommerce-customer-segmentation.git
