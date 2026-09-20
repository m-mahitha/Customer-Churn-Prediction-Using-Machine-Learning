# Customer Churn Prediction Using Machine Learning

## Project Overview

Customer churn occurs when a customer stops using a company's services. Predicting customer churn can help businesses identify customers who may leave and understand the factors associated with customer loss.
This project uses Machine Learning to predict whether a telecom customer will **churn or continue using the service** based on customer information such as tenure, contract type, services, and billing details.

## Objective

The main objective of this project is to build a Machine Learning classification model that can predict customer churn and evaluate its performance using different classification algorithms.

## Dataset

The project uses the **Telco Customer Churn Dataset**.
The dataset contains information about telecom customers, including:
- Customer demographics
- Tenure
- Services used
- Contract details
- Payment method
- Monthly charges
- Total charges
- Customer lifetime value (CLTV)
- Churn status

**Target Variable:** `Churn Label`

The target contains two classes:
- `Yes` → Customer churned
- `No` → Customer did not churn

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Machine Learning Workflow

The project follows a complete Machine Learning workflow:
1. Data Loading and Understanding
2. Data Cleaning and Preprocessing
3. Feature Preparation
4. Train-Test Split
5. Model Building
6. Model Evaluation
7. Model Comparison
8. Feature Importance Analysis
9. Final Results and Conclusion

## Machine Learning Models

Two classification algorithms were used:

### 1. Logistic Regression

Logistic Regression was used as the primary classification model for predicting whether a customer would churn or not.

### 2. Random Forest

Random Forest was used as a second classification model to compare its performance with Logistic Regression.

## Model Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 80.27% |
| Random Forest | 79.56% |

The models were evaluated using accuracy, confusion matrix, precision, recall, and F1-score.

For the churn class, Logistic Regression achieved:

- Precision: 0.68
- Recall: 0.57
- F1-score: 0.62

## Feature Importance

Feature importance was analyzed using the Random Forest model.
The top features included:
1. Tenure Months
2. Total Charges
3. Monthly Charges
4. CLTV
5. Latitude
6. Longitude
7. Internet Service - Fiber optic
8. Payment Method - Electronic check
9. Contract - Two year
10. Dependents - Yes

These features had relatively higher importance in the Random Forest model's predictions.

## Project Structure

```text
Customer-Churn-Prediction-Using-Machine-Learning/
│
├── Customer_Churn_Prediction.ipynb
├── Telco_customer_churn.csv
└── README.md
