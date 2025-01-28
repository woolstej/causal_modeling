# Predicting and Explaining Customer Churn: A Data Science Approach with Causal Inference Insights
from: https://github.com/Adesuaayo/Customer-Churn/blob/main/README.md

## Table of Contents
- [Introduction](#introduction)
- [Why Predicting Churn Matters](#why-predicting-churn-matters)
- [Data Overview](#data-overview)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Correlation and Feature Importance](#correlation-and-feature-importance)
- [Model Building](#model-building)
- [Model Performance](#model-performance)
- [Actionable Insights](#actionable-insights)
- [Conclusion](#conclusion)

## Introduction
Acquiring new customers is a never-ending game, but keeping the ones you have is pure gold. That's where customer churn prediction comes in.  By analyzing customer behavior, we can predict who's at risk of leaving and swoop in with retention strategies.  This project focuses on predicting customer churn using machine learning techniques, emphasizing causal inference to explain the relationships between features and churn.

## Why Predicting Churn Matters
Churn can significantly impact revenue and customer acquisition costs. Retaining existing customers is often more cost-effective than acquiring new ones, making churn prediction a critical business strategy.

## Data Overview
We utilized a dataset containing various customer behavior metrics, including:
- **Complaints**: Number of complaints made by customers.
- **Subscription Length**: Duration of customer subscriptions.
- **Usage**: Total minutes or seconds of service usage.
- **Frequency of Use**: How often customers utilize the service.
- **Churn**: Target variable indicating customer retention status.

## Exploratory Data Analysis (EDA)
Key findings from our EDA include:
- High complaint rates correlate with increased churn.
- Service usage patterns show that most customers have low usage, but outliers exist with high usage.
- The churn rate was found to be approximately 15.7%, highlighting the need for tailored retention strategies.

## Correlation and Feature Importance
We computed a correlation matrix and identified:
- **Complaints**: Correlation of 0.53 with churn.
- **Status**: Correlation of 0.50 with churn.

### Feature Importance
Using Random Forest and Gradient Boosting models, we determined the following feature importance:
- **Random Forest**: 
  - 1. Complaints
  - 2. Second of Use
  - 3. Frequency of Use
  - 4. Subscription Length
  - 5. Status
  - 6. Age Group
  - 7. Charge Amount
  - 8. Tariff Plan
- **Gradient Boosting**:
  - 1. Complaints
  - 2. Second of Use
  - 3. Status
  - 4. Frequency of Use
  - 5. Subscription Length
  - 6. Age Group
  - 7. Charge Amount
  - 8. Tariff Plan

## Model Building
We trained two models for churn prediction:
- **Random Forest**: Flexibility and interpretability, suitable for imbalanced datasets.
- **Gradient Boosting**: Excellent for complex patterns in data.

## Model Performance
- **Random Forest**: 
  - Accuracy: 96%
  - Precision (Churned Customers): 93%
- **Gradient Boosting**: 
  - Accuracy: 94%
  - Precision (Churned Customers): 89%

## Actionable Insights
Businesses can leverage the insights from the models to:
- **Address Complaints**: Proactive customer service strategies.
- **Tailored Offers**: For high-usage customers to re-engage them.
- **Target New Subscribers**: Focus on retention strategies for new customers.

## Conclusion
This project demonstrates the power of data-driven insights in customer churn prediction, enabling businesses to enhance retention strategies effectively.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib/Seaborn (for EDA visualizations)
