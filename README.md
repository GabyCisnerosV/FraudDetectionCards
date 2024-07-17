# FraudDetectionCards

## A) Objectives
- Learn by practice the applications of AI in fraud detection.
- Be able to detect fraud in an imbalanced dataset


## B) Description
- Fraud keeps evolving and so the alternatives to detect it should do to. In this project I try to predict credit card fraud using a dataset created using Sparkov Data Generation | Github tool (link: https://github.com/namebrandon/Sparkov_Data_Generation) created by Brandon Harris. The dataset was originally created for a Kaggle competition with this tool (https://www.kaggle.com/datasets/kartik2112/fraud-detection/data?select=fraudTrain.csv)

## C) Dataset
I selected this dataset as it offers a complete view of how the data would look when using real world data, with features like: merchant type, location of the customer, job and age of the customer, etc. Finding a non-synthetic dataset with features other than ones grouped using dimension reduction techniques like PCA is hard due to data protection of customers.

### Dataset features:
Below you can see a full description of the features from the dataset:
- Index - Unique Identifier for each row
- trans_date_trans_time - Transaction DateTime
- cc_num - Credit Card Number of Customer
- merchant - Merchant Name
- category - Category of Merchant
- amt - Amount of Transaction
- first - First Name of Credit Card Holder
- last - Last Name of Credit Card Holder
- gender - Gender of Credit Card Holder
- street - Street Address of Credit Card Holder
- city - City of Credit Card Holder
- state - State of Credit Card Holder
- zip - Zip of Credit Card Holder
- lat - Latitude Location of Credit Card Holder
- long - Longitude Location of Credit Card Holder
- city_pop - Credit Card Holder's City Population
- job - Job of Credit Card Holder
- dob - Date of Birth of Credit Card Holder
- trans_num - Transaction Number
- unix_time - UNIX Time of transaction
- merch_lat - Latitude Location of Merchant
- merch_long - Longitude Location of Merchant
- is_fraud - Fraud Flag

## D) Content
The main parts of this project are:
1) Data Cleaning and Preprocessing
2) EDA
3) Modeling
4) Comparing Results

## E) Results

## F) Next Steps
Attemp improoving results using deep learning techniques
