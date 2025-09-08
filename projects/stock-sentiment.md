---
layout: single
title: "News Sentiment & Stock Movement"
permalink: /projects/stock-sentiment/
---

# News Sentiment & Stock Movement

**Problem**  
Traders needed to integrate news sentiment into short-term stock direction prediction.

**Methods**
- Used **FinBERT** to extract sentiment from financial news.  
- Built rolling feature store with lagged stats.  
- Trained calibrated classifier with walk-forward validation.  
- Performed ablation to measure sentiment contribution.

**Results**
- Beat naive benchmarks for stock direction prediction.  
- Showed clear uplift from sentiment features.

**Business Impact**
- Stronger trading signals.  
- Better explainability of decisions.  

**Code / Repo**  
*Work-in-progress repository*
