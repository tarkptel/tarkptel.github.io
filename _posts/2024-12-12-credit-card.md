# 💳 Credit Card Approval Prediction  

![Credit Card Approval Prediction](/assets/images/images.jpg)

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/credit-card-approval-prediction)  

## 📌 Project Overview  
This project leverages **machine learning** to predict whether a credit card application will be approved or rejected based on user demographics and financial details. By analyzing key customer attributes such as **income, employment status, and credit history**, the model helps automate the approval process with high accuracy.  

## 📂 Dataset  
- **Source**: Kaggle  
- **Target Column**: **Status** (Approved/Rejected)  

## 🔍 Steps Involved  
1. **Data Cleaning** – Handled missing values and inconsistencies.  
2. **Exploratory Data Analysis (EDA)** – Discovered key patterns affecting approvals.  
3. **Feature Selection** – Identified the most important predictors.  
4. **Data Encoding** – Converted categorical variables into numerical formats.  
5. **Model Training & Evaluation** – Tested multiple ML models to find the best performer.  

## 🚀 Model Performance  

| Model            | Accuracy | F1 Score | Precision | Recall  |  
|-----------------|----------|----------|-----------|---------|  
| **Random Forest** | 98.76%   | **98.48%** | 98.30%    | 98.76%  |  
| **XGBoost**      | 98.76%   | 98.34%  | 97.98%    | 98.76%  |  
| **SVM**         | **98.91%** | 98.37%  | 97.84%    | **98.91%** |  

## 🔹 Why Random Forest?  
Although **SVM achieved the highest accuracy (98.91%)**, **Random Forest was chosen** as the final model due to its:  
- **High F1-Score (98.48%)**, ensuring a balance between Precision & Recall.  
- **Robustness against overfitting** compared to complex models.  
- **Ability to handle both categorical & numerical data** efficiently.  

## 📌 Future Improvements  
- **Deploy the model** as a web app for real-time predictions.  
- **Enhance interpretability** using SHAP (SHapley Additive Explanations).  
- **Integrate real-world financial data** for better generalization.  

