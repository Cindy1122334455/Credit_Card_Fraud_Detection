# Credit Card Fraud Detection

### Problem Overview
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The objective of this problem is to identify whether a new transaction is fraudulent or not. Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications. 

### Data Source 
The dataset for this credit card fraud detection comes from Kaggle: 

https://www.kaggle.com/mlg-ulb/creditcardfraud

### Findings
     * The data set is highly skewed which contains omly 492 frauds in a total of 284,807 observations. This resulted in only 0.172% fraud cases which makes sense in real life due to the low number of fraudulent transactions.
     * The dataset consists of numerical values from the 28 'Principal Component Analysis (PCA)' transformed features, namely V1 to V28. As such,we only need to normalize features 'Time' and 'Amount' and we do not need to perform feature engineering.
     * There is no missing value in the dataset.

### Data Modeling
I perfromed Auto-encoder model using both tensorflow and keras. After using oversampling method SMOTE to make data balanced, I used Logistic Regression as the baseline model and then improved this baseline model via Logistic Regression with Grid Search, Random Forest, Random Forest with Grid Search, LightGBM model and Xgboost model.
