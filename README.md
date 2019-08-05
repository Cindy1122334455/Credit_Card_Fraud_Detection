# Credit Card Fraud Detection

### Problem Overview
The Credit Card Fraud Detection Problem includes modeling past credit card transactions with the knowledge of the ones that turned out to be fraud. This model is then used to identify whether a new transaction is fraudulent or not. Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications. In this kernel we will use various predictive models to see how accurate they are in detecting whether a transaction is a normal payment or a fraud. 

### Data Source 
The dataset for this credit card fraud detection comes from Kaggle: 
https://www.kaggle.com/mlg-ulb/creditcardfraud

### Findings
*     The data set is highly skewed which contains omly 492 frauds in a total of 284,807 observations. This resulted in only 0.172% fraud cases which makes sense in real life due to the low number of fraudulent transactions.

*     The dataset consists of numerical values from the 28 'Principal Component Analysis (PCA)' transformed features, namely V1 to V28. As such,we only need to normalize features 'Time' and 'Amount' and we do not need to perform feature engineering.

*     There is no missing value in the dataset.

### Data Modeling
I perfromed Autoencoder model usikng both tensorflow and keras framework. After using oversampling method SMOTE to make data balanced, I used Logistic Regression as the Baseline Model, Logistic Regression with Grid Search, Random Forest, Random Forest with Grid Search, LightGBM model and Xgboost model.
