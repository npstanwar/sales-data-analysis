# 🛒 E-commerce Sales & Behavior Analysis

This project analyzes a large e-commerce event dataset (56 million rows) to understand customer behavior and identify key drivers of revenue. The goal is to move beyond simple reporting to uncover actionable insights.


### Analysis Workflow:
1.  **Data Cleaning & Preparation:** Efficiently load and clean the 56M row dataset using vectorized operations.
2.  **Sales Performance Analysis:** Identify top products, brands, and categories driving revenue.
3.  **Behavioral Funnel Analysis:** Correctly model the user conversion funnel (View → Cart → Purchase) on a session basis.
4.  **Cart Abandonment Insights:** Analyze *which* products are most frequently left in abandoned carts.
5.  **Customer Retention (Cohort Analysis):** Track user cohorts to understand customer loyalty and retention over time.
6.  **Predictive Modeling:** Build a RandomForest model to predict the likelihood of a user making a purchase based on their browsing behavior.

### Libraries & Tools Used
* **Data Manipulation:** pandas, numpy
* **Data Visualization:** matplotlib, seaborn
* **Machine Learning:** scikit-learn (specifically RandomForestClassifier)
* **Environment:** Jupyter Notebook

### Key Findings & Conclusion
The analysis and predictive model revealed that a user's engagement with the cart is the most significant signal of purchase intent.

**Feature Importance for Predicting Purchase:**
* view_to_cart_ratio: 33.4%
* unique_brands_carted: 20.6%
* unique_categories_carted: 20.2%
* total_carts: 16.8%
* avg_price_carted_items: 7.3%

**Conclusion:** The strongest predictor of a future purchase is a user's past engagement with the cart. Users who add many different items, brands, and categories to their cart, and who have a high view-to-cart ratio, are a strong signal of purchase intent.


