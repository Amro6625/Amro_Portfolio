---
layout: single
title: "UK Road Traffic Accident Analysis (2020)"
permalink: /projects/uk-accidents/
---

# UK Road Traffic Accident Analysis (2020)

**Problem**  
Analyse UK accident data to find severity drivers and predict likelihood.

**Methods**
- Used SQL to extract/clean large datasets.  
- Analyzed accident frequency by time/day (found **20% Friday increase**).  
- Detected anomalies with **LOF**, finding **5% outliers**.  
- Applied K-Means clustering → **10 high-risk areas**.  
- Built stacked ML model (RF + GBM + Logistic).  

**Results**
- Prediction accuracy **74%** (stacking).  
- Balanced metrics: accuracy 68%, precision 70%, recall 65%.  
- Forecasted **15% reduction** possible with law enforcement at peak hours.

**Business Impact**
- Supported safety campaigns (e.g. youth road safety).  
- Guided resource deployment at junctions/high-risk times.  
- Insights informed policy recommendations.


**Code:** [https://github.com/Amro6625/Accident_Project-.git](https://github.com/Amro6625/Accident_Project-.git)
