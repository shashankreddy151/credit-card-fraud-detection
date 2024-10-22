# **Fraudulent E-Commerce Transactions Dataset**

## **Description**
The **Fraudulent E-Commerce Transactions** dataset is a synthetic dataset created to simulate transaction data from an e-commerce platform, with a focus on fraud detection. It contains features commonly found in transactional data, along with engineered attributes to aid in developing and testing fraud detection algorithms. The dataset is fully synthetic and generated for educational and research purposes.

---

## **Dataset Overview**
- **Version 1 Transactions:** 1,472,952  
- **Version 2 Transactions:** 23,634  
- **Number of Features:** 16  
- **Percentage of Fraudulent Transactions:** ~5%

---

## **Features**
| Feature Name         | Description                                                                           |
|----------------------|---------------------------------------------------------------------------------------|
| `Transaction ID`      | Unique identifier for each transaction.                                               |
| `Customer ID`         | Unique identifier for each customer.                                                  |
| `Transaction Amount`  | The total amount of money exchanged in the transaction.                               |
| `Transaction Date`    | The date and time when the transaction took place.                                    |
| `Payment Method`      | The method used to complete the transaction (e.g., credit card, PayPal, etc.).        |
| `Product Category`    | The category of the product involved in the transaction.                              |
| `Quantity`            | Number of products involved in the transaction.                                       |
| `Customer Age`        | The age of the customer making the transaction.                                       |
| `Customer Location`   | The geographical location of the customer.                                            |
| `Device Used`         | The type of device used to make the transaction (e.g., mobile, desktop).              |
| `IP Address`          | The IP address of the device used for the transaction.                                |
| `Shipping Address`    | The address where the product was shipped.                                            |
| `Billing Address`     | The address associated with the payment method.                                       |
| `Is Fraudulent`       | A binary indicator of whether the transaction is fraudulent (`1` for fraudulent, `0` for legitimate). |
| `Account Age Days`    | The age of the customer’s account in days at the time of the transaction.             |
| `Transaction Hour`    | The hour of the day when the transaction occurred.                                    |

---

## **Purpose**
The dataset is designed for the following purposes:
- **Fraud Detection Model Development:** Train and test machine learning models for fraud detection in e-commerce transactions.
- **Exploratory Data Analysis (EDA):** Perform EDA to uncover patterns and trends in transactional and fraud data.
- **Feature Engineering:** Create new features based on the existing attributes to improve model performance.
- **Benchmarking Algorithms:** Use the dataset for benchmarking various fraud detection algorithms and techniques.

---

## **Generation Method**
This dataset was synthetically generated using Python's **Faker** library, along with custom logic to simulate realistic transaction patterns and fraudulent scenarios. It is not based on real individuals or transactions and was created solely for research and educational use.

---

## **File Formats**
- **Version 1 File:** `ecommerce_transactions_v1.csv`  
- **Version 2 File:** `ecommerce_transactions_v2.csv`

---

## **Usage**
To use the dataset, simply load the CSV file into your preferred data analysis or machine learning tool. Below is an example of how to load it using Python:

```python
import pandas as pd

# Load the dataset
df = pd.read_csv('ecommerce_transactions_v1.csv')

# Display first few rows
print(df.head())
