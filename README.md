# Logistic-Regression--Credit-Card-Fraud-Detection-Finance-
Predict Credit Card Fraud Using Logistic Regression

### Executive Summary
This project utilized a Logistic Regression model to predict the likelihood of fraudulent credit card transactions. By analyzing transaction data, including features like transaction amount, payment type, and account balances, the model was trained to distinguish between legitimate and fraudulent transactions. The model achieved an accuracy of approximately 83% on test data, effectively identifying patterns associated with fraudulent activity.

### Project Objective
The primary goal of this project was to develop a predictive model using Logistic Regression to detect fraudulent credit card transactions. By analyzing a dataset of 1,000 simulated transactions, the objective was to identify patterns that distinguish fraudulent transactions from legitimate ones. This model aims to provide a robust method for financial institutions to mitigate the risk of fraud and protect customer assets.

### Importance of the Final Report
Credit card fraud is a significant global issue, resulting in billions of dollars in losses each year. The final report of this project provides critical insights into the factors that contribute to fraudulent activities. By identifying these factors, financial institutions can implement more effective preventive measures, ensuring greater security for their customers. The model developed in this project not only enhances fraud detection capabilities but also contributes to reducing the overall financial impact of fraud on both customers and companies.

### Methodology
#### Data Collection
The dataset used in this project, transactions_modified.csv, contains 1,000 records of simulated credit card transactions. Each transaction is characterized by multiple features, such as the transaction amount, account balances, and the type of transaction (e.g., payment, cash out).

### Dataset Overview:
- Total Transactions: 1,000
- Fraudulent Transactions: Identified through the isFraud column.

### Key Features:
- amount: The value of the transaction.
- isPayment: Indicates if the transaction was a payment or debit.
- isMovement: Indicates if the transaction involved a transfer or cash out.
- accountDiff: The absolute difference between the origin and destination account balances.
![Dataset Preview](![Dataset Preview](https://github.com/Feyisayo0g/Logistic-Regression---Credit-Card-Fraud-Detection-Finance-/blob/main/Screenshot%202024-08-26%20at%2020.30.05.png)

### Data Analysis
#### Feature Engineering:
- Created binary columns isPayment and isMovement to capture the nature of the transactions.
- Calculated the difference between origin and destination balances (accountDiff) as a potential indicator of fraud.

#### Data Splitting:
- The dataset was split into training (70%) and testing (30%) sets using train_test_split to evaluate the model's performance.

#### Normalization:
- Applied StandardScaler to normalize the feature data, ensuring that the model treats each feature on an equal scale.

#### Model Training and Evaluation:
- Trained a Logistic Regression model on the training data.
- Evaluated the model's accuracy on both training and test sets.
- Analyzed the coefficients of the model to understand the importance of each feature in predicting fraud.

### Goals of Analysis
- Identify Key Predictors of Fraud: Determine which features most significantly contribute to detecting fraudulent transactions.
- Evaluate Model Performance: Measure the accuracy of the Logistic Regression model in predicting fraudulent activities.
- Provide Actionable Insights: Develop recommendations for improving fraud detection processes based on the model's findings.

### Results
- Model Accuracy: The Logistic Regression model achieved an accuracy of approximately 84% on both the training and test datasets.
- Key Predictors: The amount of the transaction and whether it was a movement (transfer or cash out) were the most significant predictors of fraud.
- Model Predictions: When applied to new transaction data, the model correctly identified non-fraudulent transactions, with probabilities ranging between 0.99 and 0.63 for being legitimate.

### Conclusion and Recommendations
The Logistic Regression model developed in this project demonstrates a strong ability to distinguish between fraudulent and non-fraudulent credit card transactions. However, there is room for improvement, particularly in handling imbalanced datasets, which is common in real-world scenarios.

### Recommendations:
- Enhance Model with Additional Features: Incorporate more features related to transaction history, customer behavior, and geographic data to improve model accuracy.
- Implement Real-Time Fraud Detection: Deploy the model in a real-time monitoring system to detect and prevent fraudulent transactions as they occur.
- Further Analysis on Imbalanced Data: Investigate methods such as SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance issues in larger datasets.

By implementing these recommendations, financial institutions can significantly reduce the risk of fraud, safeguarding both their assets and their customers.
