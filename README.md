# credit-card-fraud-detection-xgboost

*Dataset: Please download the dataset here: https://www.kaggle.com/datasets/kartik2112/fraud-detection?datasetId=817870&sortBy=voteCount

*Project Pipeline
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
