# Telco Customer Churn Analysis

This project analyzes customer churn data from a telecommunications company.

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
