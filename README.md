# Telco Customer Churn Analysis

## Overview

This project aims to analyze customer churn for a telecommunications company using the Telco Customer Churn dataset from Kaggle. The goal is to identify key drivers of churn and develop strategies to improve customer retention.

## Problem Statement

Customer churn is a critical issue for telecommunications companies. This project seeks to identify factors that influence customer churn and build a predictive model to estimate the probability of churn. The target metric is the churn rate, which represents the percentage of customers who cancel their service.

## Data Source

The dataset used in this project is the Telco Customer Churn dataset, available on Kaggle: [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)

## Methodology

1.  **Data Acquisition:** Downloaded the dataset from Kaggle.
2.  **Data Cleaning:** Handled missing values, converted data types, and prepared the data for analysis.
3.  **Exploratory Data Analysis (EDA):** Visualized feature distributions and relationships with churn using Pandas, Matplotlib, and Seaborn.
4.  **Feature Engineering:** Created tenure groups to improve model performance.
5.  **Predictive Modeling:** Trained and evaluated Logistic Regression, Random Forest, and Gradient Boosting models using Scikit-learn.
6.  **Model Evaluation:** Assessed model performance using accuracy, precision, recall, F1-score, AUC-ROC, confusion matrices, and ROC curves.

## Exploratory Data Analysis (EDA)

- Month-to-month contracts have a significantly higher churn rate.
- Customers with shorter tenure are more likely to churn.
- Fiber optic internet service is associated with higher churn.
- Gender has minimal impact on churn.
- The dataset exhibits class imbalance, with more non-churned customers.

## Predictive Modeling

- **Models Used:** Logistic Regression, Random Forest, Gradient Boosting.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, AUC-ROC, Confusion Matrix, ROC Curve.
- **Results:**

  ```
  Metrics for Logistic Regression:
    Accuracy: 0.7882
    Precision: 0.6226
    Recall: 0.5160
    F1-score: 0.5643
    AUC-ROC: 0.7014

  Metrics for Random Forest:
    Accuracy: 0.7775
    Precision: 0.6063
    Recall: 0.4652
    F1-score: 0.5265
    AUC-ROC: 0.6779

  Metrics for Gradient Boosting:
    Accuracy: 0.7889
    Precision: 0.6296
    Recall: 0.5000
    F1-score: 0.5574
    AUC-ROC: 0.6968
  ```

- **Feature Importance:** Contract type, tenure, and internet service are among the most influential features.
- **Best Model:** Logistic Regression had the highest AUC-ROC score, and also the best F1 score, therefore it is the best model. Gradient Boosting had the highest accuracy.

## Results and Insights

- Logistic Regression and Gradient Boosting performed the best.
- Month-to-month contracts, short tenure, and fiber optic internet service are significant drivers of churn.

## Recommendations

- Offer longer-term contracts with discounts to reduce churn among month-to-month customers.
- Implement targeted retention programs for customers with short tenure.
- Improve customer support and service quality for fiber optic internet users.
- Consider offering bundled services or loyalty programs.

## Future Work

- Perform hyperparameter tuning to improve model performance.
- Explore additional feature engineering techniques.
- Address class imbalance using oversampling or undersampling.
- Create an interactive dashboard using Tableau or Power BI.
- Deploy the model for real-time churn prediction.

## Installation and Usage

1.  Clone the repository: `git clone
2.  Install required dependencies: `pip install pandas numpy scikit-learn matplotlib seaborn`
3.  Run the Jupyter notebooks in the `notebooks/` directory.

Key Takeaways from the Graphs:

Contract Type: Month-to-month contracts are a significant driver of churn.
Tenure: Shorter tenure is associated with higher churn.
Internet Service: Customers with fiber optic internet service are more likely to churn.
Total Charges and Monthly Charges: These numerical features are correlated and may influence churn.
Gender: Gender does not seem to be a large factor in churn.
Data Imbalance: The dataset is imbalanced, with more non-churned customers.

We have created a logistic regression model, a random forest model, and a gradient boosting model to predict customer churn. The logistic regression model has an accuracy of 0.7882, the random forest model has an accuracy of 0.7775, and the gradient boosting model has an accuracy of 0.7889. The gradient boosting model has the highest accuracy and precision, but the logistic regression model has the highest recall. The logistic regression model has the highest F1-score, and the random forest model has the highest AUC-ROC score.

Metrics for Logistic Regression:
Accuracy: 0.7882
Precision: 0.6226
Recall: 0.5160
F1-score: 0.5643
AUC-ROC: 0.7014
Metrics for Random Forest:
Accuracy: 0.7775
Precision: 0.6063
Recall: 0.4652
F1-score: 0.5265
AUC-ROC: 0.6779
Metrics for Gradient Boosting:
Accuracy: 0.7889
Precision: 0.6296
Recall: 0.5000
F1-score: 0.5574
AUC-ROC: 0.6968

## Dataset

The dataset used is the Telco Customer Churn dataset from Kaggle.

## Folder Structure

- `data/`: Contains the dataset.
- `notebooks/`: Contains Jupyter notebooks for analysis.
- `scripts/`: Contains Python scripts for data processing.
- `visualizations/`: Contains visualizations (plots, charts).
- `documentation/`: Contains project documentation.
