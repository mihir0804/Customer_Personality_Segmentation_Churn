# Customer Personality Analysis, Segmentation, and Churn Prediction

This project performs an in-depth analysis of a marketing campaign dataset to understand customer personalities and behaviors. The primary goals are to segment customers into distinct groups and to predict customer churn.

## Project Overview

The project follows a standard data science workflow:
1.  **Data Cleaning and Preprocessing**: Handled missing values, standardized categorical features, and engineered new features like `TotalSpend`, `Age`, and `Customer_Lifetime`.
2.  **Exploratory Data Analysis (EDA)**: Visualized demographic distributions, analyzed product spending patterns, and investigated campaign responses to uncover initial insights.
3.  **Customer Segmentation**: Used K-Means clustering to group customers into four distinct segments based on their socio-demographic and behavioral data. PCA was used to visualize these clusters.
4.  **Churn Prediction**: Developed and evaluated three machine learning models (Logistic Regression, Random Forest, and XGBoost) to predict customer churn, using campaign response as a proxy for churn.

## Key Findings

### Customer Segments

The analysis identified four key customer segments:
*   **High-Value Loyal Customers**: High-income, high-spending customers who are highly responsive to campaigns.
*   **Potential Loyalists**: Younger customers with moderate income and spending who have the potential to become high-value.
*   **At-Risk Customers**: Low-income, low-spending customers with a high churn probability.
*   **New Customers**: Recent customers with low spending who are still in the early stages of their lifecycle.

### Churn Prediction

The XGBoost model performed the best in predicting churn, with high accuracy and AUC score. The most important features for predicting churn were found to be `Recency`, `TotalSpend`, and `Income`.

## Business Recommendations

Based on the analysis, the following recommendations are proposed:
*   **Personalized Marketing**: Tailor marketing campaigns to the specific needs and preferences of each customer segment.
*   **Loyalty Programs**: Implement loyalty programs to retain high-value customers.
*   **Reactivation Campaigns**: Target at-risk customers with special offers to prevent churn.
*   **Effective Onboarding**: Develop a strong onboarding process for new customers to encourage engagement and spending.

## How to Use

The entire analysis is contained in the `customer_analysis.ipynb` Jupyter notebook. To run the notebook, you will need to have Python and the necessary libraries installed. You can install the required libraries by running the first cell of the notebook:
```
!pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```
