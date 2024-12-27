# Customer_Segmentation_Task2

# Customer Segmentation Using K-Means Clustering

## Project Overview
This project focuses on customer segmentation using the **K-Means Clustering Algorithm**. By analyzing a dataset containing customer attributes such as **Age**, **Gender**, **Annual Income**, and **Spending Score**, we identify distinct groups of customers with similar behaviors. These insights can help businesses target marketing campaigns effectively, improve customer engagement, and optimize resource allocation.

---

## Dataset Description

The dataset contains the following columns:

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Male or Female.
- **Age**: Customer age in years.
- **Annual Income ($)**: Customer's annual income in USD.
- **Spending Score (1-100)**: A score assigned to the customer based on their spending patterns.

---

## Steps Followed in the Analysis

### 1. Data Preprocessing
- Converted categorical variable (**Gender**) to numerical values (Male = 0, Female = 1).
- Selected features: **Age**, **Gender**, **Annual Income ($)**, and **Spending Score**.
- Scaled the data using **StandardScaler** for better clustering performance.

### 2. K-Means Clustering
- Determined the optimal number of clusters using the **Elbow Method**.
- Applied K-Means with 5 clusters (as identified from the elbow method).
- Assigned each customer to a cluster and added the cluster labels to the dataset.

### 3. Visualization

#### **Cluster Analysis**

1. **Annual Income vs Spending Score**:
   - Scatter plot visualizing clusters based on income and spending patterns.
   - Insights:
     - High-income, high-spending customers were clearly identifiable (Cluster 1).
     - Low-income, high-spending customers formed a separate group (Cluster 2).

2. **Age vs Spending Score**:
   - Scatter plot showing customer segmentation based on age and spending behavior.
   - Insights:
     - Younger customers tended to have higher spending scores (Clusters 2 and 3).
     - Older customers showed moderate spending behavior (Cluster 0).

---

## Cluster Characteristics

| Cluster | Age   | Annual Income ($) | Spending Score | Description                                         |
|---------|-------|--------------------|----------------|-----------------------------------------------------|
| 0       | 55.28 | 47.62             | 41.71          | Older, moderate income, moderate spenders.          |
| 1       | 32.88 | 86.10             | 81.53          | High-income, high-spending young customers.         |
| 2       | 25.77 | 26.12             | 74.85          | Low-income, high-spending younger customers.        |
| 3       | 26.73 | 54.31             | 40.91          | Moderate-income, low-spending younger customers.    |
| 4       | 44.39 | 89.77             | 18.48          | High-income, low-spending middle-aged customers.    |

---

## Key Insights

1. **Cluster 1**: High-income, high-spending customers are valuable. Focus on retention through personalized marketing and loyalty programs.
2. **Cluster 2**: Young, low-income customers with high spending habits. Target them with affordable and appealing offers.
3. **Cluster 4**: High-income, low-spending customers represent untapped potential. Engage them with targeted campaigns to increase spending.
4. **Clusters 0 & 3**: Moderate to low spenders. Incentivize with discounts or bundled offers.
