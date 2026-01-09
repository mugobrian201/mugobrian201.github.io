---
title: "Nepal Earthquake Damage Prediction"
date: 2024-05-15
importance: 1
categories: [Disaster Response, Classification]
tags: [Python, Scikit-learn, Logistic Regression, Decision Trees]
image: /assets/images/nepal-project-thumb.jpg
description: "Predicted building damage severity from the 2015 Nepal earthquake to optimize emergency response"
---

{% include figure image_path="/assets/images/nepal-project-visual.jpg" alt="Nepal earthquake damage prediction visualization" caption="Feature importance analysis showing key predictors of structural damage" %}

### Project Overview
Developed a machine learning model to predict building damage severity following the 2015 Nepal earthquake, enabling efficient resource allocation during disaster response. This project demonstrates how data science can save lives in vulnerable communities.

### Technical Implementation
- **Data Preparation**: Created automated wrangling function to handle 38+ features including building materials, floor counts, and geographic location
- **Model Development**:
  - Logistic Regression baseline model (74% accuracy)
  - Optimized Decision Tree Classifier with hyperparameter tuning (78% accuracy)
  - Utilized walk-forward validation for time-series robustness
- **Key Techniques**: Ordinal encoding for categorical features, Gini importance analysis, residual diagnostics

### Impact & Insights
Identified that buildings with **mud mortar** and **4+ floors** were 3.2x more likely to suffer severe damage. These insights can directly inform:
- Targeted retrofitting programs in earthquake-prone regions
- Emergency response prioritization protocols
- Building code reforms in developing nations

### Technologies Used
{% include icon.html icon="fab fa-python" title="Python" %}
{% include icon.html icon="fas fa-project-diagram" title="Scikit-learn" %}
{% include icon.html icon="fas fa-chart-line" title="Statsmodels" %}
{% include icon.html icon="fab fa-github" title="GitHub" %}

[View Full Notebook](https://github.com/mugobrian201/portfolio/blob/main/nepal_earthquake_damage_prediction.ipynb){: .btn .btn--info}
[Explore Dataset on Kaggle](https://www.kaggle.com/datasets/crgrimm/nepal-earthquake-damage){: .btn .btn--info}
