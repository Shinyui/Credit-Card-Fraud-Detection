# Credit-Card-Fraud-Detection
Classify anonymized credit card transactions as fraudulent or genuine

## Project Description
This project is dedicated to classify anonymized credit card transactions as fraudulent or genuine via various machine learning & data sciecne technique.


## Dataset Source
This dataset is originally published by **Machine Learning Group - ULB** via Kaggle. The dataset can be downloaded from [here](https://www.kaggle.com/mlg-ulb/creditcardfraud)

## Dataset Context
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

## Dataset Description
The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Experiments Taken
Logistic Regression w/ different threshold 


## Steps Taken
1. Dropped feature *Time*
2. train_test_split
3. Subsampling (due to imbalanced dataset)
4. Standardized feature *Amount*
5. Modeling via *Logistic Regression* w/ *L2 Regularization*

## Final Model & Result
Logistic Regression w/ *L2 Regularization* and *Threshold as 0.73*

|        |     | 0         | 1         |
| ------ | --- | --------- | --------- |
| Actual | 0   | 83966     | 1341      |
| Actual | 1   | 10        | 126       |
|        |     | Predicted | Predicted |
