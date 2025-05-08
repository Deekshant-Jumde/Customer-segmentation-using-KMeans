📊 Overview
Objective: To identify different segments of customers to better understand their behavior and target them effectively.

Dataset: The dataset contains information about customer demographics (Age, Gender, Annual Income) and spending patterns.

Technique Used: K-Means Clustering (Unsupervised Learning)

🧠 Key Steps
Data Preprocessing and Visualization

Optimal Cluster Selection using the Elbow Method

K-Means Model Training

Cluster Visualization and Analysis

📌 Tools & Libraries
Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

📈 Outcome: Insights from Clustering
After applying K-Means clustering on the dataset, the following key insights and outcomes were derived:

1. Segmentation Based on Annual Income Alone
When clustering was done using Annual Income (k$) as a standalone feature:

The optimal number of clusters was found using the elbow method, where the inertia value significantly dropped at k=3.

The model categorized customers into three income groups:

Low-income group

Middle-income group

High-income group

However, this segmentation did not account for spending behavior, limiting its business value.

2. Segmentation Based on Income & Spending Score
A more insightful clustering was achieved by using both Annual Income and Spending Score:

The elbow method suggested k=5 as the optimal number of clusters.

This segmentation revealed five distinct customer types:

High income, high spending – Valuable customers for loyalty programs.

High income, low spending – Potential customers for targeted promotions.

Low income, high spending – Possibly impulsive buyers; opportunity for upselling.

Low income, low spending – Budget-conscious segment.

Moderate income and spending – Average, stable customers.

3. Demographic Analysis of Clusters
The clusters were further analyzed based on gender distribution:

Each cluster had a mix of male and female customers, with some variation in proportions.

For example, the cluster with low income and high spending had a higher percentage of female customers.

The average age in each cluster also varied, revealing patterns like:

Younger customers tend to spend more irrespective of income.

Older customers often had higher incomes but varied spending habits.

4. Standardized Clustering for Accuracy
Features were standardized using StandardScaler for better clustering accuracy.

K-Means was then applied to the scaled data, and the elbow method again confirmed 5 optimal clusters, reinforcing earlier findings.

🔍 Business Value
This segmentation allows businesses to personalize marketing:

Offer premium services to high-value customers.

Engage low-spending high-income customers with discounts or incentives.

Tailor budget offers for low-income high-spending segments.

It also supports customer retention, campaign planning, and resource allocation for maximum ROI.

