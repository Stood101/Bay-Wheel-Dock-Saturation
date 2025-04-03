# 🚲 Bay Wheels Dock Saturation Analysis

This project analyzes dock saturation in the **Bay Wheels** bike-sharing service in San Francisco. Dock saturation occurs when a docking station is completely full, preventing users from returning their bikes. This analysis combines **exploratory data analysis** and **predictive modeling** to understand and anticipate saturation events.

## 📌 Objectives

- Identify temporal and weather-based patterns that influence dock saturation
- Build classification models to predict saturation events
- Evaluate model performance and recommend operational improvements

## 📊 Dataset Features

The dataset includes:
- Time-based features: `hour`, `day of week`, `month`, `season`
- Environmental features: `temperature (°C)`, `humidity`, `wind speed`, `visibility`, `UV index`, `precipitation`
- Target variable: `saturated` (1 = dock full, 0 = dock not full)

## 🔍 Analysis Highlights

- **EDA** shows clear peaks in saturation during morning and evening commute hours
- Saturation is highly seasonal, with **summer and fall** showing higher saturation rates
- **Correlation analysis** reveals temperature, hour, and UV index are positively related to saturation
- **Feature importance** from Random Forest confirms temperature, hour, and humidity as top predictors

## 🤖 Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

All models were evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## 📁 Files

- `Bundel_Himanshu_A2.ipynb`: Jupyter notebook with full analysis
- `Bundel_Himanshu_A2.html`: Exported HTML version of the notebook
- Dataset: included in repo `bikes.xlsx`

## ✅ Conclusion

Random Forest and Gradient Boosting models achieved the best results with over **92% F1 score**, proving reliable in predicting dock saturation. Findings suggest that operational planning should focus on **warm-weather months and peak commute hours** to reduce user frustration and maintain system reliability.

