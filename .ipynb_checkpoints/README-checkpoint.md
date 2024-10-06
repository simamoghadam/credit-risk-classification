# credit-risk-classification

## Overview of the Analysis

The goal of this analysis is to create a supervised machine learning model that can predict if a loan is safe (class 0) or risky (class 1). I chose logistic regression, a method used to make decisions between two options. The data used for this model includes details like loan amount, interest rate, borrower’s income, debt, and more. The aim was to predict whether a loan will be healthy (0) or high-risk (1). The dataset contains 77,500 rows of information in a CSV file.

Steps in the Process:

* The data has splited into labels (loan status: healthy or risky) and features (the other details about the loan).
* The data was then divided into training and testing sets.
* We created a Logistic Regression model, which helps in predicting two outcomes: healthy or risky.
* The model was trained using the training data.
* We used the test data to make predictions.
* Finally, we evaluated how well the model performed using accuracy, precision, and recall scores.


## Results
Model Performance:

Accuracy: The model is 99% accurate, meaning it correctly predicts 99% of the loans.

Precision (correct predictions):

Healthy Loan (Class 0): 1.00 (100% correct)
High-Risk Loan (Class 1): 0.85 (85% correct)

Recall (capturing actual cases):

Healthy Loan (Class 0): 0.99 (99% correct)
High-Risk Loan (Class 1): 0.91 (91% correct)


## Summary

The logistic regression model is excellent at predicting healthy loans (class 0), with perfect precision (1.00) and nearly perfect recall (0.99). For risky loans (class 1), it does a good job too, with a precision of 0.85 and recall of 0.91.

However, the model struggles a bit more with risky loans because there are fewer examples of them in the data (only 619 high-risk loans compared to 18,765 healthy ones). Adding more high-risk loans to the dataset could help improve the model's ability to predict them.

Since preventing risky loans is more important than just predicting healthy ones (because a defaulted loan can cause more loss), this model does a good job overall, with an accuracy of 99%.