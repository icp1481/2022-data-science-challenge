# 2022 Data Science Project - KAIST-POSTECH-UNIST Competition (Silver Award)

This repository contains methodology for our award-winning project in the **2nd KAIST-POSTECH-UNIST Data Science Competition**, where we received the **Silver Award**. Our project focused on **predicting small business owners** and optimizing advertisement strategies based on user behavior.

## Project Overview

Our goal was to develop a **machine learning model** that accurately identifies **small business owners** based on their login and transaction behaviors. We further extended our analysis to optimize **pop-up advertisement strategies** for maximizing expected profit.

### Achievements
- **Silver Award** in KAIST-POSTECH-UNIST Data Science Competition
- **Highest AUC-ROC Score** achieved with **CatBoost** model
- **Profit Optimization** by selecting the best threshold and strategy for ad targeting

---

## 📊 Task Breakdown

### Task 1: Small Business Owner Prediction
#### Approach:
- **Exploratory Data Analysis (EDA)**
  - Time series visualization to identify behavior patterns
  - Feature engineering based on login & transaction periodicity
- **Model Selection**
  - Tested **XGBoost, LightGBM, CatBoost, AdaBoost, GradientBoost, Stacking Classifier**
  - **Best model:** **CatBoost** with AUC-ROC of **0.899**
- **Key Features Used**
  - Login/transaction frequency over different time periods
  - Behavior patterns before/after holidays & weekends
  - Peak activity trends (e.g., end-of-month spikes)

### Task 2: Pop-up Advertisement Planning
- **Expected reward per correct business prediction: ₩500,000**
- **Pop-up cost per attempt: ₩400**
- **Profit Matrix-Based Optimization**
  - Selected optimal **decision threshold** through theoretical and experimental analysis
  - **Best Model:** **CatBoost (Threshold = 0.08, Expected Profit = ₩175,955)**

### Task 3: Expected Profit & Strategy
- **Two strategies for ad targeting**
  - **Strategy 1:** Train a separate login prediction model
  - **Strategy 2:** Directly use business probability for ad selection
- **Final Decision:** **Strategy 2** resulted in the highest expected profit of **₩114,090,750**

---

## 📈 Results & Key Insights
- **Feature Engineering is crucial** for improving AUC-ROC scores
- **Stacking models** helped improve predictive performance
- **Time-based behavior analysis** significantly contributed to identifying small business owners
- **Profit-driven decision making** led to an **optimized ad strategy**

---

## 🛠️ Tech Stack & Libraries
- **Python, Pandas, NumPy, Scikit-Learn, LightGBM, CatBoost, XGBoost**
- **Matplotlib, Seaborn** for data visualization
- **Feature Engineering & Model Optimization** techniques applied

