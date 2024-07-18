# FraudDetectionCards 💳🚨

## Objectives 🎯
- Gain practical experience with AI applications in fraud detection.
- Understand and address the unique challenges of detecting fraud.
- Explore strategies for handling imbalanced datasets in machine learning.
- Build and evaluate various models to detect credit card fraud.
- Identify key features that indicate fraudulent activity in credit card transactions.

## Description 📄
Fraud is constantly evolving, and the detection methods to identify it must evolve as well. In this project, I aim to predict credit card fraud using a dataset generated with the [Sparkov Data Generation](https://github.com/namebrandon/Sparkov_Data_Generation) tool created by Brandon Harris. This dataset was originally created for a [Kaggle competition](https://www.kaggle.com/datasets/kartik2112/fraud-detection/data?select=fraudTrain.csv).

To handle data imbalance, I employ undersampling techniques and test different machine learning models, including Random Forest Classifier and XGBoost. I use k-fold cross-validation to identify the best model and then compare the results of the top-performing models.

## Content 📚
The main parts of this project are:
1. Data Cleaning, Preprocessing, and Exploratory Data Analysis (EDA)
2. Handling Data Imbalance
3. Modeling
4. Comparing Models

## Dataset 📊
I chose this dataset as I believe it provides a comprehensive view of what real-world data might look like, including features such as merchant type, customer location, job, and age. Finding a non-synthetic dataset with such detailed features is challenging due to customer data protection.

### Dataset Features:
Here is a full description of the features from the dataset:
- **Index** - Unique Identifier for each row
- **trans_date_trans_time** - Transaction DateTime
- **cc_num** - Credit Card Number of Customer
- **merchant** - Merchant Name
- **category** - Category of Merchant
- **amt** - Amount of Transaction
- **first** - First Name of Credit Card Holder
- **last** - Last Name of Credit Card Holder
- **gender** - Gender of Credit Card Holder
- **street** - Street Address of Credit Card Holder
- **city** - City of Credit Card Holder
- **state** - State of Credit Card Holder
- **zip** - Zip Code of Credit Card Holder
- **lat** - Latitude Location of Credit Card Holder
- **long** - Longitude Location of Credit Card Holder
- **city_pop** - Credit Card Holder's City Population
- **job** - Job of Credit Card Holder
- **dob** - Date of Birth of Credit Card Holder
- **trans_num** - Transaction Number
- **unix_time** - UNIX Time of Transaction
- **merch_lat** - Latitude Location of Merchant
- **merch_long** - Longitude Location of Merchant
- **is_fraud** - Fraud Flag

## Results 📈
After applying Random Forest and XGBoost, these are the results:

**Comparison of Best Models:**

| Model         | Accuracy | Precision | Recall  | F1 Score | ROC AUC |
|---------------|----------|-----------|---------|----------|---------|
| Random Forest | 0.926425 | 0.945886  | 0.902054| 0.923450 | 0.926040|
| XGBoost       | 0.979534 | 0.976939  | 0.981569| 0.979249 | 0.979566|

The features that appear to be most relevant for predicting fraud are:
- Amount of transaction
- Hour of the day
- Industry of the merchant (especially distinguishing between internet shopping, grocery stores, and gas stations)

## Next Steps 🚀
- Try using LightGBM (LGBM) as it is commonly used in many fraud identification cases.
- Attempt to improve results using deep learning techniques.
