# XAI-Interpretable-ML Assignment: Customer Churn Prediction

## Overview

This project involves predicting customer churn for a telecommunications company using various machine learning models. The goal is to identify patterns and factors contributing to customer churn and to select the most effective model for prediction.  

Dataset used: [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?resource=download)

## Exploratory Data Analysis (EDA)

Before building the models, EDA was conducted to understand the dataset better:
- **Data Loading**: The dataset was loaded and examined for missing values and data types.
- **Feature Analysis**: Distribution and summary statistics of numerical features (`tenure`, `MonthlyCharges`, `TotalCharges`) were analyzed.
- **Categorical Feature Analysis**: Distribution of categorical features were analyzed.
- **Correlation Analysis**: Examined correlations between features and the target variable (`Churn`).
- **Visualizations**: Histograms, bar plots, and heatmaps were used to visualize the data distributions and relationships.

## Data Preparation

- **Preprocessing**: Standardized numerical features and one-hot encoded categorical features.
- **Train-Test Split**: Data split into training (80%) and test (20%) sets.

## Models

### 1. Linear Regression
- **Train Accuracy**: 80.30%
- **Test Accuracy**: 79.18%
- **Metrics**:
  - **Train MSE**: 0.1383
  - **Test MSE**: 0.1459
  - **Train R²**: 0.2913
  - **Test R²**: 0.2522
- **Takeaways**: The linear regression model provides a basic understanding of feature impacts but struggles with capturing complex patterns.

![image](https://github.com/user-attachments/assets/e2a60cfd-815c-4792-ad8c-9ed81d49ce76)


### 2. Logistic Regression
- **Train Accuracy**: 80.85%
- **Test Accuracy**: 78.82%
- **Takeaways**: Logistic regression offers better accuracy and interpretability than linear regression, making it a good choice for binary classification tasks.

![image](https://github.com/user-attachments/assets/e7cb9039-46ed-4462-8af8-b57f74b6dde2)


### 3. Generalized Additive Model (GAM)
- **Train Accuracy**: 81.33%
- **Test Accuracy**: 79.60%
- **Takeaways**: GAM performed the best in modeling non-linear relationships and provides detailed insights into feature impacts for this dataset.

![image](https://github.com/user-attachments/assets/9c27e10c-5bed-44f9-9bbc-5bb49182adf1)

## Conclusion

- **Linear Regression**: Provides a basic understanding but limited by its linear assumptions.
- **Logistic Regression**: Offers improved accuracy and interpretability.
- **GAM**: Best performance with the ability to capture complex, non-linear relationships, making it the recommended model for predicting customer churn.

## Credits

Used Claude AI for assistance with creating visualizations and comments.
