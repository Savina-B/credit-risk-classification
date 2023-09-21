# Module 12 Report Template

# Overview of the Analysis:

Building machine learning models to forecast loan outcomes based on financial data is the goal of this investigation. The purpose of the data, which comprises of characteristics of loan applications, is to forecast whether a loan is healthy (0) or high-risk (1). The stages of the analysis are as follows:

Data preparation involves importing the data, preparing it, and encoding categorical variables as well as addressing missing values.

Create models using machine learning to forecast the results of loans. There were made two models:

Model 1 is a logistic regression model that was developed using the initial data.

Model 2: A logistic regression model that was trained using the RandomOverSampler on oversampled data.

Model Evaluation: Analysing both models' performance using metrics like recall, accuracy, precision, and F1-score.

# Results:

Machine Learning Model 1: Logistic Regression (Original Data)

Balanced Accuracy Score: 0.94
Precision (Label 0 - Healthy Loan): 1.00
Recall (Label 0 - Healthy Loan): 1.00
Precision (Label 1 - High-Risk Loan): 0.86
Recall (Label 1 - High-Risk Loan): 0.91

Machine Learning Model 2: Logistic Regression (Oversampled Data)

Balanced Accuracy Score: 0.96
Precision (Label 0 - Healthy Loan): 1.00
Recall (Label 0 - Healthy Loan): 0.99
Precision (Label 1 - High-Risk Loan): 0.85
Recall (Label 1 - High-Risk Loan): 0.99

# Summary:
Other machine learning models performed well in forecasting loan outcomes:

For high-risk loans, Model 2 (Logistic Regression with Oversampled Data) performs better than Model 1 in terms of balanced accuracy and recall. For high-risk loans, it obtained a balanced accuracy score of 0.96 and a recall score of 0.99, showing that it accurately identified almost all of them while retaining a solid balance of precision.

Model 1 (Logistic Regression with Original Data) also did well, with a recall for high-risk loans of 0.91 and a balanced accuracy score of 0.94. With a precision and recall of 1, it performed exceptionally well at predicting good loans.

The particular challenge and its priorities will determine which model is used. Model 2 is advised due to its greater recall rate for high-risk loans if accurately identifying high-risk loans is the primary issue (Label 1). However, Model 1 may be favoured if precision and memory for healthy loans (Label 0) are equally important because it perfectly balanced precision and recall for healthy loans.

The organization's risk tolerance and the proportional costs of false positives and false negatives may influence the model selection in practise. Depending on the particular requirements of the challenge, both models can be taken into consideration for deployment as they have both shown great performance.



