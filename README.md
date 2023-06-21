# Project Overview
The main goal of Credit Card Fraud Detection is to effectively distinguish fraudulent transactions from a vast number of credit card transactions. This is achieved by constructing a predictive model using historical transaction data. The objective is to detect all instances of fraud while minimizing the occurrence of false alarms.


1. Data: highly imbalanced, with only 0.172% of observations being fraudulent.
2. 28 transformed features (V1 to V28) and two untransformed features (Time and Amount).
3. No missing data in the dataset


- Generally, our aim is to maximize the recall while limiting the False Positive Rate (FPR). However, it is possible to misclassify a significant number of charges and still maintain a low FPR, thanks to the presence of numerous true negatives.
- This encourages the selection of a comparatively lower threshold, leading to a high recall but exceptionally low precision.


- When training a model with a balanced dataset, it enhances the performance on the validation data.
- Nevertheless, the objective is to optimize performance on the imbalanced production dataset. Ultimately, it is crucial to strike a balance that yields the best results in production.
- One approach to address this issue is to utilize all fraudulent transactions and selectively subsample non-fraudulent transactions as required to achieve the desired target rate.
