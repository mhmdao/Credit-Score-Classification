# 🏦 Credit Score Classification
## 📌 Overview
The company has collected basic bank details and gathered a lot of credit-related information. This project focuses on **predicting credit scores** based on financial and demographic data, which implies the probability of loan default. A credit score is a crucial factor used by financial institutions to assess the creditworthiness of an individual. This project leverages machine learning techniques to classify individuals into different credit score categories.

## 🎯 Objective
- ✅ The purpose of this project is to build an intelligent system to segregate the people into credit score brackets to reduce the manual efforts.
- ✅ Perform **Exploratory Data Analysis (EDA)** to understand key factors affecting credit scores.
- ✅ Build a **classification model** to predict credit scores.
- ✅ Evaluate model performance using various metrics (accuracy, precision, recall, F1-score).
- ✅ Deploy the model for potential real-world applications (if applicable).

- **Source:** [Kaggle - Credit Score Classification](https://www.kaggle.com/datasets/parisrohan/credit-score-classification)
- **Files Used:** `train.csv`
- **Size:** ~100,000 records
- **Main Features:**
  - `ID`: Unique identifier
  - `Customer_ID`: Unique customer ID
  - `Month`: Data collection month
  - `Age`: Age of the customer
  - `Occupation`: Employment type
  - `Annual_Income`: Reported yearly income
  - `Monthly_Inhand_Salary`: Estimated monthly salary
  - `Num_Bank_Accounts`: Total bank accounts
  - `Num_Credit_Card`: Number of credit cards
  - `Interest_Rate`: Rate charged on loans
  - `Delay_from_due_date`: Days delayed in loan payments
  - `Credit_History_Age`: Length of credit history
  - `Monthly_Balance`: End-of-month account balance
  - `Credit_Score` (Target variable): **Poor**, **Standard**, or **Good**

## 📜 Dataset License
The dataset used in this project is provided under the 
[CC0 1.0 Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/) license.  
This means the dataset is free to use, modify, and distribute without restrictions.

## 🏗️ Tech Stack
- **Programming Language:** Python
- **Libraries Used:**
  - **Data Processing & Analysis:** Pandas, NumPy
  - **Visualization:** Matplotlib, Seaborn
  - **Machine Learning:** Scikit-learn

## 🛠️ Project Workflow

### **1️⃣ Data Preprocessing and Exploratory Data Analysis (EDA)**
- Exploring data and features
- Encoding categorical features
- Distribution of credit scores
- Correlation between income, bank accounts, and credit score
- Impact of delayed payments on credit score

### **2️⃣ Model Development**
- Tried different classification models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
- Evaluated using:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix

### **3️⃣ Results & Insights**
- **Feature Importance**: Outstanding Debt, Late Payments and interest rates significantly impact credit scores.
- **Best Model:** Gradient boosting achieved the highest accuracy (~87%).
- **Key Finding:** Customers with less outstanding debt and less interest rate tend to have **Good** credit scores. Secondly, people with middle range values of debt has a higher probability of poor credit score / more chance of loan default, which is likely because of other features such as salary or interest rate. Secondly, while the top 9 features significantly impact predictions, the sum of the 15 less important features also plays a crucial role in predicting the credit score based on the shap values. Therefore, they should not necessarily be removed from the model.

## 🚀 How to Run
```bash
# Clone this repository
git clone https://github.com/mhmdao/credit-score-classification.git

# Navigate to the project folder
cd credit-score-classification



