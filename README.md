# Macroeconomic Inflation Modeling & Prediction  
Machine Learning & Time-Series Analysis (India)

This repository contains Python code and a comprehensive analysis of **macroeconomic inflation dynamics in India** using RBI time-series data. The project applies **exploratory data analysis, time-series feature engineering, supervised learning, and unsupervised clustering** to predict near-term inflation and uncover structural inflation regimes.

---

## Project Objectives

### Inflation Trend Analysis
- Analyze historical CPI inflation trends using monthly RBI data.
- Examine inflation persistence through lagged variables and rolling averages.

### Macroeconomic Indicator Analysis
- Study the relationship between inflation and key macroeconomic variables:
  - Money Supply (M3 Growth)
  - Exchange Rate (USD/INR)
  - Index of Industrial Production (IIP Growth)
  - Interest Rates (Call Money Rate)

### Inflation Prediction
- Forecast **near-term inflation** by predicting the **three-month rolling average of CPI inflation**.
- Apply supervised machine learning models for short-term inflation forecasting.

### Inflation Regime Identification
- Identify distinct inflation regimes (low, moderate, high) using unsupervised learning.
- Analyze regime persistence and structural shifts in inflation behavior.

---

## Dataset

**Source:** Reserve Bank of India (RBI)  
**Frequency:** Monthly

The dataset contains macroeconomic indicators including:

- `Date`: Observation month  
- `Inflation_Rate`: CPI inflation (%)  
- `M3_Growth`: Money supply growth (%)  
- `USD_INR`: Exchange rate (INR per USD)  
- `IIP_Growth`: Industrial production growth (%)  
- `Call_Money_Rate`: Weighted average call money rate (%)  

Derived features:
- Lagged inflation variables
- Lagged macroeconomic indicators
- Three-month rolling average of inflation (target variable)

---

## Methodology

### Exploratory Data Analysis (EDA)
- Inflation trend visualization
- Correlation heatmaps
- Distribution analysis
- Multicollinearity inspection

### Feature Engineering
- Lag-based features to capture inflation persistence
- Rolling averages to smooth short-term volatility
- Feature standardization for clustering and ML models

### Supervised Learning (Inflation Prediction)
**Models Used:**
- Random Forest Regressor
- XGBoost Regressor

**Target Variable:**
- Three-month rolling average of CPI inflation

**Forecast Results:**
- Random Forest predicted next 3-month average inflation ≈ **2.78%**
- XGBoost predicted next 3-month average inflation ≈ **3.15%**

### Unsupervised Learning (Inflation Regime Analysis)
**Techniques Used:**
- K-Means Clustering
- Hierarchical Clustering

**Validation Methods:**
- Elbow Method (WCSS)
- Dendrogram analysis

**Outcome:**
- Identification of structurally distinct inflation regimes
- Evidence of regime persistence over time

---

## Key Findings

- Inflation shows strong **temporal persistence**, making lagged features critical.
- Short-term inflation forecasting improves using smoothed (rolling average) targets.
- Inflation behavior is **regime-dependent**, varying across economic conditions.
- Combining supervised prediction with regime analysis enhances interpretability.

---

## Tools and Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost

---

## Project Structure

