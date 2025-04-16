---
title: "🍽️ Food Demand Forecasting"
date: 2025-04-15
categories: [Projects]
tags: [Machine Learning, Hugging Face]
---

### 🌟 Project Overview  
Food demand forecasting is a critical aspect of managing supply chain operations, particularly for meal providers, restaurants, or food delivery services. **This project focuses on predicting the number of orders for meals** in a given week, helping businesses optimize their inventory and operations. <br><br>

### 🌟 Problem Statement
Predicting the demand for meals in advance helps businesses prepare for fluctuating demand, optimize inventory, reduce food waste, and improve customer satisfaction. The goal of this project is to forecast the number of orders for a specific meal in a specific center for the upcoming week. <br><br>

### 🔗 Links  
- 🔥 **Live Demo:** [Try the App](https://huggingface.co/spaces/tarkpatel/food-demand-forecast)  
- 🛠 **GitHub Repo:** [View on GitHub](https://github.com/tarkptel/Food-Demand-Forecasting)  <br><br>

### 📦 Approach and Methodology
Data Collection:
The dataset includes historical orders for different meal centers with features like `week`, `meal_id`, `center_id`, `checkout_price`, `base_price`, and promotional flags such as `emailer_for_promotion` and `homepage_featured`. <br><br>

### 🎯 Feature Engineering:  
**"Data Science is not about choosing the right model, it's about choosing the right features"** So, To improve prediction accuracy, several features i created, such as:
- `week_sin`, `week_cos` – Encode week cyclically to capture seasonality.
- `demand_lag_1`, `demand_lag_2` – Demand in previous 1 and 2 weeks.
- `rolling_mean_3` - 3-week rolling mean of demand.
- `rolling_std_3` – 3-week rolling standard deviation of demand.
- `price_diff` - Difference between base price and checkout price.
-  `price_ratio` - Ratio of checkout price to base price.
- `meal_avg_demand` - Average demand for each meal across all centers.
- `center_meal_avg` - Average demand for each meal in a specific center.
- `quarter` - Week converted into quarter (0 to 3).
- `weeks_since_event` - Weeks passed since a reference point (e.g. week 100).
- `normalized_week` - Week normalized based on first week of each meal.
- `is_promo` - Whether emailer or homepage promotion is active.
- `promo_effect` - Combined effect of promotion and price difference.
- `price_per_center` - Average checkout price per center.
- `meal_popularity_in_center` - 	Meal popularity within a specific center.
- `center_id_encd`, `meal_id_ecd` - Encoded categorical features for center and meal IDs. <br><br>

### 🏆 Model Selection:
Two models were trained to compare performance:

- Random Forest (RF)
- XGBoost (XGB)

After evaluating both, **XGBoost** was chosen due to its better performance in handling this forecasting task.

### 🚀 Deployment Details:
- **User Inputs:** Users can select the week, center ID, meal ID, checkout price, and promotion flags.
- **Prediction:** Based on the input values, the model forecasts the number of orders for the meal in the given week.
