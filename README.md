# Anomaly Detection in Transactions
 - Anomaly detection in transactions means identifying unusual or unexpected patterns within transactions or related activities. These patterns, known as anomalies or outliers, deviate significantly from the expected norm and could indicate irregular or fraudulent behaviour.

## What is its usecase?
 - This is particularly valuable in the financial sector, where it can help combat fraud and ensure the security of user accounts. Here's a breakdown of its key usecase:
    - **Fraud Detection:**
       - By analyzing vast amounts of transaction data, anomaly detection systems can learn typical spending habits of users. This includes factors like average transaction amount, 
         frequency of purchases, and typical merchant locations.
       - When a transaction deviates significantly from these patterns, for instance, a sudden large purchase or a transaction from an unfamiliar location, the system can flag it as               potentially fraudulent.
       - This allows financial institutions to take immediate action, such as contacting the user for verification or blocking the transaction. This can significantly reduce financial             losses due to fraudulent activities.

## Data Description
 - I have used the `transaction_anomalies_dataset.csv` file for the project
 - The dataset contains information about various financial transactions, each represented by several features:
  1. Transaction_ID: Unique identifier for each transaction.
  2. Transaction_Amount: The monetary value of the transaction.
  3. Transaction_Volume: The quantity or number of items/actions involved in the transaction.
  4. Average_Transaction_Amount: The historical average transaction amount for the account.
  5. Frequency_of_Transactions: How often transactions are typically performed by the account.
  6. Time_Since_Last_Transaction: Time elapsed since the last transaction.
  7. Day_of_Week: The day of the week when the transaction occurred.
  8. Time_of_Day: The time of day when the transaction occurred.
  9. Age: Age of the account holder.
  10. Gender: Gender of the account holder.
  11. Income: Income of the account holder.
  12. Account_Type: Type of account (e.g., personal, business).
  
## Model Description
 - The model I have used is IsolationForest, you can check the model's training process in the `anomaly_detection.ipynb` notebook

## Libraries Used
 - Pandas
 - Matplotlib
 - Seaborn
 - Scikit-learn

## Evaluation Metrics
 - Precision:
     Normal: 1.00
     Anomaly: 1.00
 - Recall:
    Normal: 1.00
    Anomaly: 1.00
 - Accuracy: 1.00


