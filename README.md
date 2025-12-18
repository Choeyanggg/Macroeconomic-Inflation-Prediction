Macroeconomic Inflation Modeling & Prediction

Machine Learning & Time-Series Analysis (India)

This repository contains Python code and a comprehensive analysis of macroeconomic inflation dynamics in India using RBI time-series data. The project combines exploratory data analysis, time-series feature engineering, supervised learning, and unsupervised clustering to forecast near-term inflation and identify structural inflation regimes.

Project Objectives
Inflation Trend Analysis

Analyze historical CPI inflation trends using monthly RBI data.

Study inflation persistence through lagged variables and rolling averages.

Macroeconomic Indicator Analysis

Examine the relationship between inflation and key macro variables such as:

Money supply (M3 growth)

Exchange rate (USD/INR)

Industrial activity (IIP growth)

Interest rates (Call Money Rate)

Inflation Prediction

Forecast near-term inflation by predicting the three-month rolling average of CPI inflation.

Evaluate supervised machine learning models for short-term inflation forecasting.

Inflation Regime Identification

Identify distinct inflation regimes (low, moderate, high) using unsupervised learning.

Analyze regime persistence and structural differences in inflation behavior.

Dataset

Source: Reserve Bank of India (RBI)
Frequency: Monthly macroeconomic time-series data

The dataset includes the following variables:

Date: Observation month

Inflation_Rate: CPI inflation (%)

M3_Growth: Money supply growth (%)

USD_INR: Exchange rate (INR per USD)

IIP_Growth: Index of Industrial Production growth (%)

Call_Money_Rate: Weighted average call money rate (%)

Derived features:

Lagged inflation variables

Lagged macroeconomic indicators

3-month rolling average of inflation (target variable)

Methodology
Exploratory Data Analysis (EDA)

Trend analysis of CPI inflation

Correlation heatmaps and multicollinearity checks

Distribution analysis of macroeconomic variables

Visualization of inflation behavior over time

Feature Engineering

Lag-based features to capture inflation persistence

Rolling averages to smooth short-term noise

Standardization of features for clustering and ML models

Supervised Learning (Inflation Prediction)

Models Used:

Random Forest Regressor

XGBoost Regressor

Target Variable:

Three-month rolling average of CPI inflation

Forecast Results:

Random Forest predicted next 3-month average inflation ≈ 2.78%

XGBoost predicted next 3-month average inflation ≈ 3.15%

Unsupervised Learning (Regime Analysis)

Techniques Used:

K-Means Clustering

Hierarchical Clustering

Validation Tools:

Elbow Method (WCSS)

Dendrogram analysis

Outcome:

Identification of distinct inflation regimes

Evidence of regime persistence and structural shifts

Key Findings

Inflation exhibits strong temporal persistence, making lag-based features critical for forecasting.

Short-term inflation prediction benefits from modeling smoothed trends rather than single-month values.

Inflation behavior is regime-dependent, varying across economic phases.

Combining supervised prediction with regime analysis improves interpretability and economic insight.

Tools and Libraries Used

Python

pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

Project Structure
├── inflation_analysis.ipynb      # Jupyter notebook with EDA, modeling, and visualizations
├── rbi_macro_data.xlsx           # RBI macroeconomic dataset
└── README.md                     # Project documentation

Conclusion

This project demonstrates how machine learning and time-series analysis can be applied to macroeconomic data to improve inflation forecasting and interpretation. Rather than focusing solely on model accuracy, the analysis emphasizes inflation persistence, structural regimes, and economic interpretability, providing a more realistic approach to macroeconomic forecasting.
