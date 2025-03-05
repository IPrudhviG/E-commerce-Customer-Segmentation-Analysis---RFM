# RFM-Based Customer Segmentation using K-Means

## 📌 Project Overview
This project applies **Recency, Frequency, and Monetary (RFM) analysis** with **K-Means clustering** to segment customers based on their purchasing behavior. The goal is to identify different customer groups to help businesses implement targeted marketing strategies and improve customer retention.

## 📊 Dataset
- The dataset consists of transactional data from an online retail store.
- Key fields used:
  - **Customer ID**: Unique identifier for each customer.
  - **Invoice Date**: The date of each purchase.
  - **Invoice No**: Unique transaction identifier.
  - **Quantity**: Number of items purchased.
  - **Unit Price**: Price per item.
  - **Total Price**: Derived as `Quantity * Unit Price`.

## 🔢 RFM Analysis
**RFM (Recency, Frequency, Monetary) analysis** helps segment customers based on their transaction history:
- **Recency (R)**: How recently the customer made a purchase.
- **Frequency (F)**: How often the customer makes purchases.
- **Monetary Value (M)**: How much money the customer spends.

## 📌 Methodology
1. **Data Preprocessing**:
   - Handling missing values.
   - Removing duplicate records.
   - Computing `Total Price` for each transaction.
2. **RFM Score Calculation**:
   - Extracting the most recent transaction date.
   - Computing Recency (days since last purchase), Frequency (total transactions), and Monetary value (total spending per customer).
3. **Scaling Data**:
   - Standardizing RFM values using Min-Max scaling.
4. **Applying K-Means Clustering**:
   - Determining the optimal number of clusters using the **Elbow Method**.
   - Applying **K-Means clustering** on the RFM dataset.
5. **Visualizing Customer Segments**:
   - Scatter plots to analyze clusters.
   - Bar charts to interpret segment behavior.

## 📈 Key Results
- Customers are segmented into distinct groups based on purchasing behavior.
- High-value customers are identified for loyalty programs.
- Infrequent buyers are recognized for re-engagement campaigns.

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- **VS Code - Jupyter Notebook** for development
- **GitHub** for version control

