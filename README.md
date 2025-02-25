"# Credit-risk_analysis" 
predicting credit default risk using a machine learning approach(Random Forest). The dataset contains various financial and demographic attributes of individuals, and the goal is to classify whether a person will default on their credit payment or not.

DATASET
https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients
The dataset consists of multiple financial indicators, including credit limit, past bill amounts, and payment statuses.
Class-0: No defaults 
Class-1: Default in payments

DATA PREPROCESSING
Removed the first row from the dataset.
Renamed the target column to loan_default.
Handled missing values by dropping null entries.

#Used a Random Forest Classifier with 100 estimators.

Accuracy achieved is 81%
Class 0 (No Default): Precision - 84%, Recall - 94%
Class 1 (Default): Precision - 63%, Recall - 36%
The model performs well in identifying non-defaulters but struggles with identifying defaulters.

![image alt](https://github.com/pulipakav1/Credit-risk_analysis/blob/420129d8250e19c2c62fce5d40b14ec4593381e4/Classification%20Report.png)

The model is biased towards predicting No Default (Class 0).
It misclassifies many defaulters (Class 1) as non-defaulters.

![image alt](https://github.com/pulipakav1/Credit-risk_analysis/blob/420129d8250e19c2c62fce5d40b14ec4593381e4/confusion%20matrix.png)

Important Features are:
PAY_0 (Repayment Status for the Most Recent Month)
ID (Unique Identifier, may not be relevant and should be removed)
AGE
BILL_AMT1 (Latest Bill Amount)
LIMIT_BAL (Credit Limit)

![image alt](https://github.com/pulipakav1/Credit-risk_analysis/blob/420129d8250e19c2c62fce5d40b14ec4593381e4/Feature%20importance.png)


Further Improvements
XGBOOST/ CNN
