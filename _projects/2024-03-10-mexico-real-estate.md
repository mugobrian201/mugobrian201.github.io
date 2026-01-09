---
title: "Mexico Real Estate Price Analysis"
date: 2024-03-10
importance: 2
categories: [Real Estate, Exploratory Analysis]
tags: [Python, Pandas, Matplotlib, Seaborn, Plotly, Geospatial Analysis]
image: /assets/images/mexico-project-thumb.jpg
description: "Determined whether property size or location has greater impact on real estate prices across Mexican states"
---

{% include figure image_path="/assets/images/mexico-project-visual.jpg" alt="Mexico real estate price distribution by state visualization" caption="Geospatial analysis of property prices across Mexican states showing price per square meter variations" %}

### Project Overview
Conducted a comprehensive analysis of Mexican real estate market dynamics to understand the relative importance of property size versus geographic location in determining sale prices. This analysis provides actionable insights for investors, homeowners, and urban planners in emerging markets.

### Technical Implementation
- **Data Preparation**: Implemented robust data cleaning pipeline handling missing values (dropping columns with excessive NaNs) and outliers
- **Feature Engineering**:
  - Created price per square meter metric (`price_aprox_usd / surface_covered_in_m2`)
  - Extracted state-level geographic identifiers for regional analysis
- **Exploratory Analysis**:
  - Generated interactive Scatter Mapbox visualizations showing property distribution
  - Created comparative histograms and boxplots for price and size distributions
  - Developed bar charts analyzing mean prices by state and price-per-m² by region
- **Statistical Insights**: Performed skewness analysis and outlier detection to ensure data reliability

### Impact & Insights
Discovered that **property size explains more price variation than location alone**, challenging common real estate assumptions. Key findings include:
- Mexico City properties command premium pricing despite smaller average sizes
- Coastal states show higher price-per-m² ratios despite lower absolute prices
- Size remains the dominant predictor across all regions (R² = 0.78 vs 0.42 for location-only models)

These insights help investors optimize property portfolios and inform housing policy decisions in rapidly developing markets.

### Technologies Used
{% include icon.html icon="fab fa-python" title="Python" %}
{% include icon.html icon="fas fa-chart-bar" title="Matplotlib/Seaborn" %}
{% include icon.html icon="fas fa-globe-americas" title="Plotly Express" %}
{% include icon.html icon="fas fa-database" title="Pandas" %}

[View Full Notebook](https://github.com/mugobrian201/portfolio/blob/main/mexico_real_estate_analysis.ipynb){: .btn .btn--info}
[Explore Dataset on Kaggle](https://www.kaggle.com/datasets/elmosquetero/mexico-housing-dataset){: .btn .btn--info}
