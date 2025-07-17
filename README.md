# credit-card-fraud-detection-xgboost

# Project Overview
This project aims to develop a robust and accurate credit card fraud detection system using XGBoost. The dataset used in this project contains transactional data, with features that describe the transactions and labels indicating whether a transaction is fraudulent.

# Dataset
The dataset is divided into two main files:
- **Training Data:** [fraudTrain3.csv](https://drive.google.com/file/d/1fr54Agfvjh_Y2urDL7UhnQ1QMGFrYdig/view?usp=sharing)
- **Testing Data:** [fraudTest3.csv](https://drive.google.com/file/d/1U8VDFneDtaFhN8IrMD_ukC9Ferp0IfDa/view?usp=sharing)


# Key Features:
- merchant: Merchant name
- category: Transaction category
- amount: Transaction amount
- cc_num: Credit card number
- first, last: Cardholder's first and last name
- gender: Cardholder's gender
- street, city, state, zip: Cardholder's address
- lat, long: Cardholder's latitude and longitude
- city_pop: Population of the city
- job: Cardholder's job
- dob: Cardholder's date of birth
- trans_num: Transaction number
- unix_time: Transaction time in Unix format
- merch_lat, merch_long: Merchant's latitude and longitude
- is_fraud: Label indicating if the transaction is fraudulent (1) or not (0)

# Steps to reproduce
1. Import Libraries: The project begins by importing essential libraries for data manipulation, visualization, and machine learning.

2. Data Collection:
- Collect Data: The dataset, sourced from Kaggle, includes simulated credit card transactions from January 1, 2019, to December 31, 2020. It consists of records from 1,000 customers and 800 merchants, providing a rich diversity of data points for analysis.
- Clean Data: Checking and handling missing values ensures data integrity.
- Feature Engineering: New feature was created to capture patterns that might indicate fraud. hour_of_day were created by converting 'unix_time' to 'transaction_time' and extract 'hour_of_day' to understand temporal patterns.

3. Exploratory Data Analysis (EDA): EDA is conducted to uncover patterns and inform feature engineering.

4. Model Training:
- Incorporating EDA Insights into Model Training
- Train-Test Split: Divide the data into 80% training and 20% testing sets. 
- Handling Imbalance: Utilize SMOTE to address class imbalance.

5. Model Evaluation: Initial evaluation of the model's performance is conducted using classification reports and confusion matrices.

6. Model Optimization and Tuning: Hyperparameter tuning is performed using RandomizedSearchCV to enhance model performance.

7. Tuned Model Evaluation: The performance of the tuned model is re-evaluated to assess improvements.
