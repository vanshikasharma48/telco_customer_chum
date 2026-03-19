# 📉 Customer Churn Prediction using Machine Learning

## 📌 Project Overview

This project predicts whether a customer will leave (churn) a telecom company using machine learning techniques. The goal is to help businesses identify customers at risk of leaving and take preventive actions.

The dataset used is the Telco Customer Churn dataset from Kaggle.

---

## 👩‍💻 Author

**Vanshika Sharma**

---

## 📊 Problem Statement

Customer churn is a major challenge for telecom companies. Losing customers leads to revenue loss.

This project builds a classification model to predict whether a customer will churn based on their demographic and service usage data.

---

## 📂 Dataset

The dataset contains information about 7000+ customers, including:

* Customer demographics (gender, senior citizen)
* Account information (tenure, contract type)
* Services (internet, phone, streaming)
* Billing details (monthly charges, total charges)

### Target Variable

* `Churn`

  * Yes → Customer leaves
  * No → Customer stays

---

## 🛠️ Technologies Used

| Tool         | Purpose              |
| ------------ | -------------------- |
| Python       | Programming          |
| Pandas       | Data manipulation    |
| NumPy        | Numerical operations |
| Seaborn      | Visualization        |
| Matplotlib   | Visualization        |
| Scikit-learn | Machine learning     |

---

## 🔎 Machine Learning Workflow

### 1️⃣ Data Loading

Dataset loaded using Pandas.

### 2️⃣ Data Cleaning

* Converted `TotalCharges` to numeric
* Handled missing values using median
* Removed unnecessary columns (customerID)

### 3️⃣ Exploratory Data Analysis (EDA)

Key insights were derived using visualization techniques.

### 4️⃣ Feature Engineering

* Converted categorical variables into numeric using one-hot encoding
* Transformed target variable (Churn) into binary format

### 5️⃣ Train-Test Split

* 80% training data
* 20% testing data

### 6️⃣ Model Training

A **Random Forest Classifier** was used due to its high accuracy and ability to handle complex relationships.

### 7️⃣ Model Evaluation

Model performance was evaluated using:

* Accuracy Score
* Classification Report

---

## 📊 Key Business Insights

* Customers with **low tenure** are more likely to churn
* **High monthly charges** increase churn probability
* **Month-to-month contracts** have the highest churn rate
* Customers with **long-term contracts (1–2 years)** are less likely to churn
* Certain payment methods (like electronic check) show higher churn

---

## 📈 Feature Importance

Top features affecting churn:

* Tenure
* MonthlyCharges
* TotalCharges
* Contract Type (Month-to-month)
* Internet Service (Fiber optic)

These features are critical for predicting customer behavior.

---

## 📊 Results

The model achieved an accuracy of approximately **78–85%**, successfully identifying customers likely to churn.

---

## 📁 Project Structure

```
churn-prediction
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── churn_project.ipynb
├── README.md
```

---

## 🚀 Future Improvements

* Hyperparameter tuning for better accuracy
* ROC-AUC analysis
* Confusion matrix visualization
* Trying advanced models like XGBoost
* Deploying the model using Streamlit

---

## 📚 Key Learnings

* Data cleaning and preprocessing
* Handling categorical variables
* Exploratory Data Analysis
* Classification models
* Feature importance interpretation
* Business-driven insights from data

---

## ⭐ Conclusion

This project demonstrates how machine learning can be used to solve real-world business problems like customer churn prediction. It combines data analysis with predictive modeling to provide actionable insights for decision-making.
