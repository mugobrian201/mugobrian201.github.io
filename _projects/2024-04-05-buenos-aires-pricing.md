---
title: "Buenos Aires Apartment Price Prediction"
date: 2024-04-05
importance: 3
categories: [Real Estate, Predictive Modeling]
tags: [Python, Scikit-learn, Linear Regression, Feature Engineering, Pipelines]
image: /assets/images/buenos-aires-project-thumb.jpg
description: "Built iterative linear regression models to predict apartment values using size and location features"
---

{% include figure image_path="/assets/images/buenos-aires-project-visual.jpg" alt="Buenos Aires apartment price prediction model performance comparison" caption="Model performance comparison showing how combining size and location features improved prediction accuracy by 37%" %}

### Project Overview
Developed a scalable predictive modeling framework for Buenos Aires apartment pricing that demonstrates the complete machine learning workflow from baseline models to production-ready pipelines. This project showcases iterative improvement methodology essential for real-world applications.

### Technical Implementation
- **Progressive Model Development**:
  - **Baseline Model**: Size-only linear regression (MAE: $12,450)
  - **Location Model**: Geographic features only (MAE: $14,230)
  - **Hybrid Model**: Combined size and location features (MAE: $8,120)
- **Advanced Techniques**:
  - Implemented Scikit-learn Pipelines for reproducible preprocessing
  - Used SimpleImputer for robust missing value handling
  - Extracted model coefficients to create interpretable prediction equations
  - Engineered price-per-area metrics for normalized comparisons
- **Validation Strategy**: Focused on iterative improvement rather than train-test split to demonstrate practical model evolution

### Impact & Insights
The hybrid model reduced prediction error by 37% compared to size-only baseline, proving that **location context significantly enhances valuation accuracy** even when size is the dominant factor. Key applications include:
- Automated property valuation tools for real estate platforms
- Investment decision support systems for portfolio optimization
- Policy analysis tools for housing affordability studies
- Foundation for mortgage underwriting algorithms

### Technologies Used
{% include icon.html icon="fab fa-python" title="Python" %}
{% include icon.html icon="fas fa-brain" title="Scikit-learn" %}
{% include icon.html icon="fas fa-project-diagram" title="Pipelines" %}
{% include icon.html icon="fas fa-chart-line" title="Plotly" %}

[View Full Notebook](https://github.com/mugobrian201/portfolio/blob/main/buenos_aires_apartment_pricing.ipynb){: .btn .btn--info}
[Explore Dataset](https://www.kaggle.com/datasets/datasets-for-projects/buenos-aires-apartment){: .btn .btn--info}
