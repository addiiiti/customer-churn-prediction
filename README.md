# Customer Churn Prediction using Machine Learning

##  Project Overview
Customer churn refers to customers leaving a service.  
This project builds a machine learning pipeline to **predict whether a customer will churn** based on their usage and account details.

The goal is to help businesses **identify high-risk customers early** and take preventive actions.

---

##  Dataset
- 20,000 customer records
- 11 features including:
  - tenure
  - monthly_charges
  - total_charges
  - contract type
  - payment method
  - internet service
- Target variable: `churn` (0 = No, 1 = Yes)

---

##  Exploratory Data Analysis
- Checked data types and missing values
- Analyzed churn distribution (imbalanced dataset)
- Studied relationships between churn and:
  - contract type
  - tenure
  - monthly charges

---

##  Data Preprocessing
- Converted numeric columns stored as strings
- Handled missing values using median imputation
- Label encoded categorical variables
- Performed train-test split to avoid data leakage
- Applied feature scaling for Logistic Regression

---

##  Models Used

### 1️⃣ Logistic Regression
- Used as a baseline model
- Required feature scaling
- Struggled to capture non-linear relationships

### 2️⃣ Random Forest Classifier
- Handles non-linearity and feature interactions
- No need for feature scaling
- Provided better recall for churned customers

---

##  Model Evaluation
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- Feature Importance analysis

---

##  Final Outcome
Random Forest performed better and was chosen as the final model.  
The model can predict churn probability for new customers.

---

##  Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Google Colab

---

##  How to Run
1. Clone the repository
2. Install dependencies  
   ```bash
   pip install -r requirements.txt
