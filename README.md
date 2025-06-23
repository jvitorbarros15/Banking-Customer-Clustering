# 🧠 Customer Segmentation using KMeans Clustering

This project performs customer segmentation using **KMeans Clustering** based on Banks customer data. The main goal is to group customers into distinct segments according to their **age**, **annual income**, and **spending score**, enabling businesses to better target their strategies.


## 📌 Project Objectives

- Discover customer groups with similar behavioral and demographic profiles
- Use unsupervised learning (KMeans) to segment customers
- Visualize clusters to support actionable business decisions



## 📁 Dataset Features

The dataset contains 200 customer records with the following attributes:

| Feature               | Description                              |
|-----------------------|------------------------------------------|
| `CustomerID`          | Unique identifier                        |
| `Gender`              | Customer gender                          |
| `Age`                 | Age of the customer                      |
| `Annual Income (k$)`  | Income in thousands of dollars           |
| `Spending Score (1-100)` | Spending behavior score assigned by the mall |



## 🔍 Exploratory Data Analysis (EDA)

- Data contains no missing values
- Customers aged between **18 and 70**
- Income ranges from **15k to 137k**
- Spending score distributed from **1 to 99**



## 📊 Clustering Methodology

1. **Feature Selection**: Focused on `Annual Income` and `Spending Score` (also used `Age` for insight).
2. **Scaling**: Standardized the features to normalize their influence.
3. **Elbow Method**: Used to determine the optimal number of clusters — result: **5 clusters**.
4. **KMeans Clustering**: Applied clustering and added labels to the dataset.
5. **Visualization**:
   - Scatter plots of feature relationships by cluster
   - Bar plots of average values per cluster

## ✅ Requirements

Install dependencies:
pip install pandas matplotlib seaborn scikit-learn

## 📈 Cluster Analysis Summary

| Cluster | Age Profile | Income Level | Spending Behavior | Insights |
|--------|-------------|--------------|-------------------|----------|
| 0      | Middle-aged | Moderate     | Moderate          | Balanced group, potential for loyalty |
| 1      | Young       | High         | Very High         | High-potential, premium customers |
| 2      | Very Young  | Low          | High              | Trend-driven, promotion-sensitive |
| 3      | Middle-aged | High         | Low               | Upsell opportunity |
| 4      | Older       | Low          | Low               | Value-conscious, low-risk group |



## 📌 Key Learnings
Even with a small set of features, unsupervised learning can extract meaningful patterns

Cluster-based segmentation allows better personalization and targeting

Visualization is essential for interpreting unsupervised model results

## 💡 Next Steps
Add more features (e.g. tenure, product usage) for deeper clustering

Deploy as a Streamlit or Dash web app for business users

Use advanced models like DBSCAN or Gaussian Mixture for comparison

## 👨‍💻 Author
João Vitor Barros da Silva
Senior Computer Science Student – Penn State
