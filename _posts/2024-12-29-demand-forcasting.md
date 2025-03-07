# 📊 Demand Forecasting Project  

## 🔍 Project Overview  
Demand forecasting is crucial for businesses to optimize inventory, reduce costs, and maximize profits. This project leverages machine learning to predict future sales based on historical data, helping businesses make data-driven decisions.  


## 1️⃣ Dataset Information  
The dataset contains sales-related attributes, including:  

- **Item ID** – Unique identifier for the item  
- **Store ID** – Unique identifier for the store  
- **Price** – Item price  
- **Week** – Week of the sale  
- **Sales** – Total units sold  

---

## 2️⃣ Exploratory Data Analysis (EDA)  
EDA was performed to uncover patterns and relationships:  

✅ **Sales trends over time**  
✅ **Correlation between price and sales**  
✅ **Seasonality patterns in sales data**  

---

## 3️⃣ Feature Engineering  
To improve model performance, additional features were created:  

- **Day, Month, and Year** – Extracted from the week column  
- **dif_bt** – Difference between `base_price` and `total_price`  
- **rd_base** – `dif_bt` divided by `base_price`  
- **rd_total** – `dif_bt` divided by `total_price`  

---

## 4️⃣ Model Selection  
Several models were tested for demand forecasting:  

- XGBoost Regression  
- Random Forest  
- **LightGBM ✅ (Chosen Model)**  
- Gradient Boost  

🔹 **LightGBM was selected for its superior efficiency and predictive accuracy.**  

---

## 5️⃣ Why LightGBM?  
✔️ **Fast training speed** and low memory usage  
✔️ **Handles large datasets efficiently**  
✔️ **Outperforms other models in predictive accuracy**  

---

## 6️⃣ Test Data Prediction  
The trained LightGBM model achieved:  

| **Metric**                 | **Score**  |  
|---------------------------|-----------|  
| **Mean Absolute Error (MAE)**  | 24.757    |  
| **R² Score**               | **0.8126**  |  

📊 **Predictions align well with actual sales trends, confirming model effectiveness.**  

---

## 🔍 Future Improvements  
🚀 **Enhancing demand forecasting for better business insights!**  

✅ **Adding External Data** – Incorporate weather, holidays, and promotions for better predictions  
✅ **Deep Learning Models** – Experiment with LSTMs or Transformers for sequential forecasting  
✅ **Hyperparameter Optimization** – Tune LightGBM with Bayesian Search for improved accuracy  
✅ **Explainability** – Use SHAP values to interpret the model’s decisions  
✅ **Real-Time Forecasting** – Implement an API to update predictions dynamically  

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/Demand-Forecasting)

---

📢 *This project is a step towards smarter demand forecasting, enabling better sales strategies and inventory management!* 🚀  
