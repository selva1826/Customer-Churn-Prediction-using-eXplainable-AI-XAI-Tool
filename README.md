# Customer Churn Prediction using XAI

## 📌 Project Overview
This project focuses on **predicting customer churn** using advanced machine learning techniques and **explainable AI (XAI)** methods. It helps businesses understand **why customers leave** and which factors contribute the most to churn.

## 🚀 Key Features
- **Churn Prediction Model**: Built using **XGBoost** for high accuracy.
- **Explainability (XAI)**: Uses **SHAP & LIME** to explain predictions.
- **User Input System**: Allows users to input customer details through an interactive selection-based UI.
- **Feature Importance Analysis**: Identifies key drivers of churn.
- **Real-time Predictions**: Generates instant predictions based on user inputs.

## 📊 Dataset Description
The dataset contains information on telecom customers, including:

| Column Name         | Description |
|---------------------|-------------|
| **Customer ID**     | Unique identifier for each customer |
| **Gender**         | Male / Female |
| **Senior Citizen** | 0 (No) / 1 (Yes) |
| **Partner**        | Yes / No |
| **Dependents**     | Yes / No |
| **Tenure**         | Number of months customer stayed with the company |
| **Internet Service** | DSL / Fiber optic / No |
| **Monthly Charges** | Amount charged monthly ($) |
| **Total Charges**  | Total amount paid by customer ($) |
| **Churn**         | Target variable (Yes / No) |

## 🏗️ Model Development
### **1️⃣ Data Preprocessing**
- **Handled missing values** by filling in appropriate values.
- **Encoded categorical variables** using Label Encoding and One-Hot Encoding.
- **Normalized numerical features** to improve model performance.

### **2️⃣ Model Training**
- Used **XGBoost** as the primary algorithm due to its efficiency and accuracy.
- Performed **Hyperparameter Tuning** to optimize performance.
- Split the dataset into **80% training and 20% testing** for validation.

### **3️⃣ Model Evaluation**
- Measured accuracy using:
  - **ROC-AUC Score**
  - **Confusion Matrix**
  - **Precision-Recall Curve**

### **4️⃣ Explainability (XAI)**
- **SHAP (SHapley Additive Explanations)**
  - Determines which features impact churn the most.
  - Provides **global interpretability** of the model.
- **LIME (Local Interpretable Model-Agnostic Explanations)**
  - Explains why a specific customer was predicted to churn.
  - Provides **local interpretability** for individual predictions.

## 🔹 How the System Works
1️⃣ The user **selects customer attributes** (e.g., tenure, internet service, charges).  
2️⃣ The trained **XGBoost model predicts churn** probability.  
3️⃣ **SHAP analysis** shows **which factors influenced the prediction**.  
4️⃣ **LIME explains** individual customer churn decisions.  

## 📌 Next Steps
- Improve accuracy with **feature engineering**.
- Deploy model as a **web API** using Flask or FastAPI.
- Create a **dashboard** in Power BI / Tableau to visualize churn trends.
- Implement **automated model retraining** to handle data drift.

---

## 🤝 Contributions
Feel free to contribute by improving the model, adding new features, or suggesting enhancements!
