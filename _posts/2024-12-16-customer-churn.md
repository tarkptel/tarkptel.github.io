# 📉 Customer Churn Prediction  

## 📌 Project Overview  
This project aims to predict customer churn using machine learning models based on customer demographics, account details, and service usage patterns. The goal is to help businesses identify high-risk customers and take proactive retention measures.  

## 📂 Data Overview  
- The dataset includes **customer demographics, account information, and service usage details**.  
- The target variable is **'Churn Label'**, indicating whether a customer has churned (Yes/No).  

## 📊 Exploratory Data Analysis (EDA)  
Key insights discovered during EDA:  
- **Customers with higher monthly charges** are more likely to churn.  
- **Long-tenured customers** have lower churn rates.  
- **Month-to-month contract holders** have the highest churn rate compared to other contract types.  

## 🛠️ Data Preprocessing  
- Handled missing values in the **'Total Charges'** column by replacing empty values with the mean.  
- Converted the **'Total Charges'** column to a numerical format (float64).  
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to address class imbalance.  

## 🔹 Feature Engineering  
Created new features to improve model performance:  
- **Tenure Buckets**: Categorized customers based on tenure duration.  
- **Monthly Charges & Total Charges Features**: Derived additional insights from spending patterns.  

## 🔹 Model Development & Evaluation  
Tested multiple machine learning models, including:  
- **Logistic Regression**  
- **Random Forest Classifier**  
- **Gradient Boosting Models (XGBoost, LightGBM)**  

### 📌 Why Random Forest?  
- Achieved the **highest F1-Score of 0.870** while maintaining robustness.  
- Handles complex datasets effectively and reduces overfitting.  
- Performs well even with limited feature engineering.  

### 📊 Model Performance (Random Forest)  

| **Metric**    | **Score** |  
|--------------|---------|  
| **Precision** | 0.857   |  
| **Recall**    | 0.808   |  
| **F1-Score**  | 0.832   |  
| **Accuracy**  | 0.823   |  
 

The balance between **Precision, Recall, and F1-Score** indicates that the model effectively minimizes false positives and false negatives.  

## 🚀 Future Improvements  
- **Deploy the model** as an interactive web app for real-time predictions.  
- **Improve interpretability** using SHAP (SHapley Additive Explanations) to explain feature importance.  
- **Test deep learning models** (e.g., Neural Networks) for potential improvements.  

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/Customer-Churn-Prediction)  

  
