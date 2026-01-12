# 📊 Customer Churn Prediction (Bank Customers)

## 📌 Project Overview
Customer churn prediction is a critical task for banks to identify customers who are likely to leave their services.  
This project uses **Artificial Neural Networks (ANN)** to predict whether a bank customer will churn based on demographic and financial information.
The goal is to help banks take **proactive actions** to retain high-risk customers.

---

## 🎯 Objective
- Identify customers who are likely to leave the bank
- Train an ANN-based binary classification model
- Analyze important features influencing customer churn

---

## 📁 Dataset
**Churn Modelling Dataset**

**Total Records:** 10,000  
**Target Variable:** `Exited`  
- `1` → Customer exited (churned)  
- `0` → Customer stayed  

### 📌 Features Used
- CreditScore  
- Geography  
- Gender  
- Age  
- Tenure  
- Balance  
- NumOfProducts  
- HasCrCard  
- IsActiveMember  
- EstimatedSalary  

---

## 🛠 Data Preprocessing
- Removed irrelevant columns:
  - `RowNumber`
  - `CustomerId`
  - `Surname`
- Encoded categorical variables:
  - **Gender** → Label Encoding using a lambda function (Male = 1, Female = 0)
  - **Geography** → One-Hot Encoding
- Applied **StandardScaler** for feature scaling
- Split data into training and testing sets (80/20)

---

## 🤖 Model Used
**Artificial Neural Network (ANN)** built using TensorFlow/Keras.

### Architecture:
- Input Layer
- Hidden Layer 1 (64 neurons, ReLU)
- Dropout (0.3)
- Hidden Layer 2 (32 neurons, ReLU)
- Dropout (0.2)
- Output Layer (1 neuron, Sigmoid) 

---
## 📈 Model Performance
- Achieved accuracy of approximately **82% – 86%**
- Evaluated using:
  - Accuracy Score
---

