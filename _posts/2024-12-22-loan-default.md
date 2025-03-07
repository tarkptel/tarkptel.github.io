# 🏦 Loan Default Prediction Project  

![Loan Default](/assets/images/la.jpg)

## 📂 Dataset Information  
The dataset contains **loan-related features**, including demographic, financial, and behavioral attributes.  

- **Total Rows:** 150,000  
- **Total Columns:** 22  
- **Target Variable:** `status` (0 = Non-Default, 1 = Default)  

## 🔧 Data Preprocessing  

### 🛠 Null Value Imputation  
Several columns had missing values and were handled as follows:  

- **Debt-to-Income Ratio (dtir1):** Imputed using the median grouped by income.  
- **Property Value (property_value), Income (income), Loan-to-Value Ratio (LTV):** Imputed using the mean.  
- **Term (term), Age (age):** Filled missing values with the most frequent value.  

### 🔢 Encoding Categorical Variables  
- **Ordinal columns** were encoded using **Label Encoding**.  
- **Age ranges** (e.g., `<25`, `45-54`, etc.) were converted to their **midpoints** for numerical representation.  

### ⚖ Handling Imbalanced Data (SMOTE)  
The target variable was highly imbalanced:  

- **Non-Default (0):** 112,031 instances  
- **Default (1):** 36,591 instances  

To balance the dataset, **SMOTE (Synthetic Minority Oversampling Technique)** was applied with `sampling_strategy=0.7`, ensuring a proportional increase in the minority class.  

## 📊 Model Selection  
Several machine learning models were evaluated, including:  

- **XGBoost Classifier**  
- **Random Forest Classifier**  
- **Gradient Boosting Classifier**  

## 🚀 Why XGBoost?  
XGBoost outperformed other models in terms of accuracy, precision, recall, and F1-score.  

### ✅ Model Performance (Before Hyperparameter Tuning)  

| **Metric**      | **Score**  |  
|----------------|----------|  
| **Accuracy**   | 91.32%   |  
| **Precision**  | 81.5%    |  
| **Recall**     | 96.7%    |  
| **F1-Score**   | 88.4%    |  
| **AUC-ROC**    | 92.1%    |  

### ✅ Final Model Performance (After Tuning)  

| **Metric**      | **Score**  |  
|----------------|----------|  
| **Accuracy**   | 91.2%    |  
| **Precision**  | 80.6%    |  
| **Recall**     | 96.6%    |  
| **F1-Score**   | 88.05%   |  
| **AUC-ROC**    | 92.3%    |  

---
## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/Loan-Default)
