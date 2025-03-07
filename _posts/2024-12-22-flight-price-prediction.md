# ✈️ Flight Price Prediction  
Utilizing machine learning to predict airfare prices with precision, this project provides insights into airfare trends based on factors like airline, travel class, departure time, and more.  

![Flight Price Prediction](/assets/images/fp3.jpeg)

## 📂 GitHub Repository  
[🔗 Link to GitHub Repo](https://github.com/tarkptel/Flight-Price-Prediction)

## 📌 Overview  
Flight prices fluctuate due to multiple factors, making prediction a complex task. This project leverages advanced machine learning models to forecast ticket prices, helping users make informed travel decisions.  

## 📊 Dataset  
The dataset includes the following key attributes:  
- **Airline**: Name of the airline  
- **Source City**: City of departure  
- **Destination City**: City of arrival  
- **Departure Time**: Categorized into Morning, Afternoon, Evening, etc.  
- **Arrival Time**: Categorized into Morning, Afternoon, Evening, etc.  
- **Stops**: Number of stops during the journey  
- **Class**: Travel class (Economy or Business)  
- **Price**: Ticket price (Target variable)  

## 🔎 Process  
To enhance model performance, the following steps were taken:  

### 🛠️ Data Preprocessing  
- **Data Cleaning**:  
  - Merged **Morning & Early Morning** into a single category.  
  - Merged **Night & Late Night** into a single category.  
- **Encoding**: Applied **One-Hot Encoding** to categorical columns like airline, source city, and destination city.  
- **Scaling**: Used **MinMaxScaler** to normalize the target column (**Price**).  
- **Feature Selection**: Retained important features such as **stops, class, and departure time**.  

### 🚀 Model Training  
Multiple machine learning models were explored:  
- **Gradient Boosting**  
- **Random Forest Regressor**  
- **XGBoost Regressor**  

Hyperparameter tuning was conducted using **RandomizedSearchCV** to optimize performance.  

## 🏆 Best Model: **XGBoost**  
XGBoost was chosen based on its superior performance in terms of evaluation metrics:  

### ✅ Model Performance  

| **Metric**                     | **Score**  |  
|---------------------------------|-----------|  
| **Mean Squared Error (MSE)**    | 0.0464    |  
| **Root Mean Squared Error (RMSE)** | 0.2156    |  
| **R² Score**                    | **0.95**  |  


📌 **Feature Importance Analysis**  
The most influential features impacting flight prices were:  
✔ **Stops**  
✔ **Class**  
✔ **Departure Time**  

### 🔍 Future Improvements  

- **Feature Engineering:** Explore additional features such as holiday seasons, demand surges, and ticket booking windows to improve accuracy.  
- **Deep Learning Models:** Implement LSTMs or Transformer-based models for better sequential trend analysis.  
- **Real-Time Price Tracking:** Integrate real-time API data to enhance model predictions based on current trends.  
- **Hyperparameter Tuning:** Further optimize hyperparameters using Bayesian Optimization for better performance.  
- **Explainability:** Use SHAP values to better interpret model decisions and improve trust in predictions.  



🚀 **Continuous improvements will ensure more precise and reliable flight price predictions!**  

---

🚀 **This project showcases how machine learning can help predict airfare trends, aiding travelers in making cost-effective booking decisions!**  
