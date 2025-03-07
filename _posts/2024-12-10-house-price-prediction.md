# 🏡 House Price Prediction  

![House Price Prediction](/assets/images/hp.jpg)

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/House-Price-Prediction/tree/main)  

## 📌 Project Overview  
Developed a machine learning model to predict house prices using various property features. The project focused on data preprocessing, feature engineering, model selection, and optimization to improve prediction accuracy.  

## 📂 Dataset Used  
- The dataset consists of various property attributes, including square footage, number of bedrooms, bathrooms, year built, and more.  
- Preprocessing steps were applied to clean and enhance data quality for better predictions.  

## 🔹 Technologies Used  
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, Seaborn  
- **Tools:** Jupyter Notebook, VS Code  

## 🔹 Data Preprocessing  
- Handled missing values using appropriate imputation techniques.  
- Identified and removed outliers to maintain data quality.  
- Applied feature scaling (standardization/normalization) to numerical columns.  

## 🔹 Feature Engineering  
- Created new features like **Total Square Footage, Total Bathrooms, House Age,** and **Years Since Remodel** to enhance model performance.  
- Introduced binary indicators for key property features (e.g., presence of a wood deck).  
- Used **Recursive Feature Elimination (RFE)** to select the most important features, improving model efficiency.  

## 🔹 Model Development & Evaluation  
- Trained multiple regression models, including **Linear Regression, Random Forest, Gradient Boosting,** and **XGBoost**.  
- Tuned hyperparameters using **RandomizedSearchCV** for optimal performance.  
- Evaluated models using **RMSE, MAE, and R² Score**, with **Gradient Boosting Regressor achieving the highest R² score of 0.89** on the test set.  

## 📊 Results & Impact  
- Feature engineering and model tuning significantly improved prediction accuracy.  
- **Gradient Boosting** was chosen for its ability to handle non-linear relationships and minimize overfitting.  
- The final model provided reliable price predictions, making it useful for real estate analysis.  

## 🔮 Future Improvements  
- Deploy the model as a web application for real-time predictions.  
- Explore deep learning models for further accuracy improvements.  
- Integrate additional external factors such as location trends and economic indicators.  

