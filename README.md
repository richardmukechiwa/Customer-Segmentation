# Customer Segmentation Using KMeans Clustering

## Project Overview

In this project, I performed customer segmentation using the KMeans clustering algorithm to identify distinct customer groups based on their Income and Total Spend. Customer segmentation is essential for businesses to better understand their customer base, allowing them to tailor marketing strategies, improve customer retention, and personalize customer experiences.

## Objectives

- Segment customers into groups based on their Income and Total Purchase Amount.
- Analyze and visualize customer behavior patterns within each segment.
- Provide actionable insights to help businesses focus on customer needs, improve services, and optimize resource allocation.

### Dataset

**Source:** Kaggle Link https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset

The dataset used in this project contains customer demographic and purchase information, including:

_Income:_ Annual income of the customer.

_Total Spend:_ Sum of the total amount spent by the customer across various product categories, including wines, fruits, meat products, fish products, sweet products, and gold products.

The dataset includes other features such as:

Recency: Number of days since the last purchase.

Kidhome/Teenhome: Number of children/teenagers in the household.

NumDealsPurchases: Purchases made with discounts or special deals.

NumWebPurchases: Number of purchases made via the website.

NumStorePurchases: Number of purchases made in physical stores.

NumCatalogPurchases: Number of purchases made via catalog.

### Feature Engineering

To improve the clustering performance, I derived:

**Total Purchase Amount:** Aggregated spend across all product categories.

Final Features Used for Clustering

- Income
- Total Purchase Amount
  
### Methodology

**Data Preprocessing:**

- Handled missing values, standardized income and purchase amount values for better performance in clustering.
- 
- Scaled both Income and Total Purchase Amount using StandardScaler to ensure that both features are on the same scale.
  
**Clustering:**

- Implemented KMeans clustering with an optimal number of clusters determined by the Elbow Method and Silhouette Score.
  
- Segmented customers into different groups based on their income levels and spending patterns.
  
**Visualization:**

- Used scatter plots and cluster centroids to visualize the customer segments.
  
- Highlighted distinct customer segments with color coding based on Income and Total Spend.
  
**Results**

The clustering analysis revealed three primary customer segments:

Here's a chart illustrating the customer segmentation results:

![Customer Segmentation Chart](C:\Users\RICH-FILES\Downloads\MachineLearning\10 portfolioprojects\Clusterpic.png)

High Income, High Spend:

Customers with the highest purchasing power and highest total spend.
Ideal for premium product marketing and loyalty programs.
Moderate Income, Moderate Spend:

Customers with moderate income and balanced spending habits.
Potential target for upselling and cross-selling opportunities.
Low Income, Low Spend:

Customers with lower income and spending.
Focus on cost-effective products and promotional deals to increase engagement.
Insights:
High-income customers tend to spend significantly more, making them prime candidates for personalized offers.
Moderate-income customers can be encouraged to increase spending by promoting higher-value products.
Low-income customers may respond better to discounts, bundles, or loyalty rewards to boost their spending behavior.
Conclusion
By segmenting customers based on income and total spend, businesses can better allocate marketing resources and create more targeted marketing campaigns. These insights can help in identifying key customer groups, improving customer satisfaction, and boosting overall sales.

Tools and Libraries
Python: Used for data preprocessing, analysis, and visualization.
Pandas: For data manipulation and feature engineering.
Scikit-learn: For implementing the KMeans algorithm.
Matplotlib/Seaborn: For creating visualizations of the clusters.
Future Work
Include more features such as recency, number of purchases by channel, and household size to further refine the segmentation.
Explore other clustering techniques like DBSCAN or Hierarchical Clustering for comparison.
Extend the analysis by incorporating predictive modeling to identify customer churn or predict future spending.


