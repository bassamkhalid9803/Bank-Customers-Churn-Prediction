# Customer Churn Prediction

This project focuses on predicting customer churn for a bank using the [Kaggle "Churn for Bank Customers" dataset](https://www.kaggle.com/datasets/mathchi/churn-for-bank-customers).

## Objective

Identify bank customers who are likely to leave (churn), based on their demographics and account activity.


## Dataset Overview

- **Filename**: `churn.csv`
- **Rows**: 10,000
- **Target**: `Exited` (1 = Customer left, 0 = Customer stayed)
- **Features**:
  - CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary


## Steps Performed

1. **Data Cleaning**  
   Dropped irrelevant columns (RowNumber, CustomerId, Surname)

2. **Encoding**  
   - `Gender`: Label Encoding  
   - `Geography`: One-Hot Encoding

3. **Feature Scaling**  
   StandardScaler applied to numerical features.

4. **Modeling**  
   Trained a `RandomForestClassifier` to predict churn.

5. **Evaluation**  
   Classification Report and Confusion Matrix.

6. **Feature Importance**  
   Visualized which features most influence churn.


## Key Insights

- Features like **Age**, **Estimated Salary**, **Balance** and **Credit Score** are important predictors.
- Random Forest provided a good balance of accuracy and interpretability.


## Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn


