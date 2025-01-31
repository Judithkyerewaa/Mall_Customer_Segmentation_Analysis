# Mall Customer Segmentation Analysis
---

![](https://github.com/user-attachments/assets/438a60f3-4042-45c6-89df-ce08608c55d9)
---

## Introduction

This project focuses on grouping a Mall’s customers into specific segments based on their spending habits, income levels, and demographics. By understanding these customer groups, the marketing team can design targeted strategies to enhance customer engagement, connect with customers, improve their shopping experience, and use resources more efficiently.



## Problem Statement

The marketing team currently employs a broad, one-size-fits-all marketing strategy, making it difficult to effectively engage customers. This project aims to address this challenge by identifying distinct customer segments based on behavioral and demographic patterns. With these insights, the marketing team can develop tailored marketing campaigns based on customers purchasing behavior and preferences, allocate resources more efficiently, and foster stronger customer relationships.


## Project Objectives

The primary objectives of this project are:

- Customer Segmentation: Group customers into meaningful clusters using demographic and behavioral data.
- Personalized Marketing Strategies: Provide actionable insights to help the marketing team design targeted campaigns.
- Resource Optimization: Focus marketing efforts on high-value customer segments to maximize return on investment (ROI).
- Enhanced Customer Relationships: Offer products and services that align with customer needs and preferences.



## Data Overview

The dataset consists of 200 unique customers, with a gender distribution of 112 females (56%) and 88 males (44%). It includes key demographic and financial information relevant to customer segmentation.

Key Data Columns:
- CustomerID – Unique identifier for each customer.
- Gender – Male or Female.
- Age – The age of the customer.
- Annual Income (k$) – Customer's yearly income in thousands of dollars.
- Spending Score (1-100) – A score reflecting the customer's spending behavior and engagement.



## Tools Used

To analyze the dataset and segment customers, we employed the following tools and techniques:

- Python – Used for data cleaning, exploratory data analysis (EDA), and clustering.
- Libraries:
  - Pandas & NumPy – Data manipulation and analysis.
  - Matplotlib & Seaborn – Data visualization.
  - Scikit-learn – Implementing clustering algorithms.
- Jupyter Notebook – Primary environment for running Python scripts and documenting analysis.



## Data Transformation

The dataset underwent a thorough cleaning process, ensuring high-quality data for analysis. There were no null values or duplicates in the data, and no data type conversions were required. The dataset was clean and ready for segmentation analysis without any preprocessing issues.



## Data Modelling
key variables for modeling, such as: Age, Annual Income (k$) and Spending Score (1-100) were used to identify patterns and group customers into clusters.

1. Scaling of Data as a results of the values in the dataset having vastly different ranges, the data was scaled or normalized using a technique like StandardScaler to ensure that all features had equal weight in the clustering process.

2. Clustering Algorithm:K-Means Clustering was applied to segment the customers.

3. The Elbow Method was used to determine the number of clusters by analyzing the sum of squared distances (inertia) for different cluster numbers.

4. After determining the ideal number of clusters ( 5 clusters), the algorithm grouped customers based on similarities in their income, age, and spending scores.



## Executive Summary
This project grouped the mall’s customers into five distinct categories based on their demographics, income, and spending habits. The goal was to find key customer groups and share insights to help improve marketing plans and better use resources.


## Overview and Findings

We identified five customer groups

![](https://github.com/Judithkyerewaa/Mall_Customer_Segmentation_Analysis/blob/main/clusters.PNG)


- Cluster 2: these are customers with high spending and high Income, our ideal customers. These customers are the best target for premium products and personalized marketing campaigns.
  
- Cluster 4: these are customers with high spending and low Income. These customers are ideal for marketing discounted products or promoting sales events.


### Other Clusters
- Cluster 0: customers with high-income and low spending; these customers need efforts to retain them.
  
- Cluster 1: Customers with moderate income and moderate spending; there is potential to encourage more spending in this group.
  
- Cluster 3: Customers with low income and low spending; these customers are less likely to contribute significantly to revenue.




## Insight Deep Dive
To better serve our customers, we grouped customers based on two key factors: annual income and spending habits. This helps the marketing team create targeted strategies for each group.

From our analysis, we identified five customer segments, but two are the most important for marketing:
 1. Cluster 2 – High-Income, High-Spending Customers (Main Target)
 2. Cluster 4 – Low-Income, High-Spending Customers (Sales & Discount Shoppers)

Cluster 2: High-Income, High-Spending Customers (Main Target)

These customers earn between $70K and $137K per year and have a high spending score (63-97), meaning they can afford and are willing to buy premium products. 54% are women, and their average age is 33 years.

### How to market to them:
- Promote luxury and high-end products with exclusive offers.
- Use personalized campaigns, such as VIP programs and loyalty rewards.
- Emphasize quality, status, and brand experience in marketing.
- Run targeted ads on luxury and lifestyle platforms.


Cluster 4: Low-Income, High-Spending Customers (Sales & Discount Shoppers)

These customers earn between $15K and $39K annually but still have a high spending score (61-99), meaning they shop frequently despite a lower income. 59% are women, and their average age is 25 years.

### How to market to this group:
- Focus on discounts, promotions, and limited-time sales.
- Highlight affordable luxury to maintain their spending habits.
- Offer installment payment plans to encourage bigger purchases.


### Spending Trends by Age

![](https://github.com/Judithkyerewaa/Mall_Customer_Segmentation_Analysis/blob/main/age_by_spending_score.PNG)


- Customers aged 20 to 40 spend the most money. Spending decreases as customers get older, suggesting the need for age-specific marketing strategies.
-  These customers can be engaged  with tech-driven shopping experiences, such as app-based promotions and interactive in-store experiences.
- Older customers tend to spend less over time, so they should be encouraged to keep shopping through loyalty rewards and incentives.




## Recommendations
To make the most of these insights, the marketing team should:

**Cluster 2 (High-Income, High-Spending Customers):**
 - Create marketing campaigns that promote luxury and high-demand products in this segment.
 - Focus promotions on female shoppers, as they make up a larger part of this group.
 - Offer personalized deals and VIP incentives to keep these valuable customers engaged.


  **Cluster 4 (Low-Income, High-Spending Customers):**
  
 - Target these customers with sales events and discounts on popular products.
 - Use value-driven promotions like buy one, get one free deals, bundle deals (buy two items together at a lower price)  to encourage them to continue shopping.


  **All Clusters:**
  
 - Use social media and digital marketing to connect with younger shoppers.
 - Implement customer loyalty programs to encourage repeat purchases across all customer groups.


  **Clusters 1, 3, and 5 (Lower Spending Customers):**
  
 - These customers do not spend as much, so they are not the main focus for now.
 - However, the marketing team could still attract them with budget-friendly promotions, loyalty rewards, and long-term engagement strategies.




## Assumptions and Caveats

### Assumptions
- The dataset includes 200 customers, and we assume this sample represents the mall’s overall customer base.
- We assume the Spending Score is a good way to measure customer engagement, even though it does not show how often they shop.
- We assume customer behavior stays consistent, but in reality, spending habits can change due to new products, price changes, or personal financial situations.




## Caveats (Limitations)
- The dataset only includes income, age, and spending score. Other important factors, like shopping frequency, customer preferences, and household size, are missing, which could improve segmentation.
- Since we analyzed only 200 customers, the results might not apply to a larger population. A bigger dataset would provide a more accurate picture of customer behavior.










