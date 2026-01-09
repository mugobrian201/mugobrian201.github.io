---
title: "Beijing Air Quality Forecasting"
date: 2024-03-25
importance: 4
categories: [Environmental Science, Time Series]
tags: [Python, Statsmodels, ARIMA, Time Series Analysis, Walk-Forward Validation]
image: /assets/images/beijing-project-thumb.jpg
description: "Time series forecasting of PM2.5 pollution levels using multiple statistical and machine learning approaches"
---

{% include figure image_path="/assets/images/beijing-project-visual.jpg" alt="Beijing PM2.5 pollution forecasting comparison" caption="Walk-forward validation results comparing Linear Regression, AR, and ARMA models for PM2.5 forecasting" %}

### Project Overview
Developed a time series forecasting system to predict dangerous PM2.5 particulate matter levels in Beijing, China. This project demonstrates advanced time series techniques with real-world applications for public health protection and environmental policy.

### Technical Implementation
- **Data Engineering**:
  - Localized timestamps using pytz for accurate temporal alignment
  - Implemented time-based resampling to daily frequency
  - Applied forward-fill imputation for missing values
  - Performed rigorous outlier removal using statistical thresholds
- **Model Development**:
  - **Linear Regression with Lag Features**: Created 1-7 day lag features for predictive modeling
  - **AutoRegressive (AR) Model**: Implemented Statsmodels AR with order selection via ACF/PACF analysis
  - **ARMA Model**: Combined autoregressive and moving average components with walk-forward validation
- **Evaluation Framework**:
  - Time-based train-test split preserving temporal sequence
  - Mean Absolute Error (MAE) as primary metric
  - Comprehensive residual diagnostics for model validation
  - Walk-forward validation for realistic performance assessment

### Impact & Insights
Surprisingly, the **Linear Regression model with lag features outperformed traditional time series models** (MAE: 12.3 vs 15.7 for ARMA), demonstrating that simpler approaches can sometimes be more effective for environmental forecasting. These predictions enable:
- Early warning systems for vulnerable populations
- Data-driven public health interventions during high-pollution events
- Policy evaluation tools for emission reduction strategies
- Urban planning insights for pollution mitigation infrastructure

### Technologies Used
{% include icon.html icon="fab fa-python" title="Python" %}
{% include icon.html icon="fas fa-microchip" title="Statsmodels" %}
{% include icon.html icon="fas fa-clock" title="Time Series" %}
{% include icon.html icon="fas fa-wind" title="Environmental Data" %}

[View Full Notebook](https://github.com/mugobrian201/portfolio/blob/main/beijing_air_quality_forecasting.ipynb){: .btn .btn--info}
[Explore Dataset on Kaggle](https://www.kaggle.com/datasets/pablomonleon/beijing-air-quality-data){: .btn .btn--info}
