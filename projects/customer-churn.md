---
layout: single
title: "Customer Churn Prediction"
permalink: /projects/customer-churn/
---


**Problem**  
Predict which customers are likely to churn next cycle so retention can intervene early (cost-sensitive framing prioritising recall on churn while controlling precision to protect ROI). 

**Data & Preparation**  
Demographics, subscribed services, contract type, payment method, tenure, billing. Cleaning, missing-value treatment, categorical encoding, selective scaling, and a leakage-safe train/validation/test split. 

**EDA Highlights (what drives churn)**  
- Highest churn: **month-to-month** contracts, **short tenure**, and **electronic check** payments.  
- Higher monthly charges and certain service bundles elevate churn risk.  
- Interaction effects (e.g., **contract × tenure**) are important → tree models capture these without manual crosses. 

**Modelling Strategy & Rationale**  
Benchmarked Logistic Regression and tree ensembles; **XGBoost** chosen for best AUC–Recall balance, non-linear interactions, and strong tabular performance. Calibrated probabilities and set an operating threshold aligned to business costs. 

**Results (hold-out test)**  
- **AUC = 0.841**, **F1 = 0.637**.  
- Key drivers (consistent across explainability views): **tenure, contract type, payment method, monthly charges**. 

**Business Impact**  
Risk scores feed CRM; prioritise top deciles first; A/B test to quantify uplift and refine thresholds/offers by micro-segment. 

**Deployment & Monitoring**  
Batch scoring (daily/weekly) with versioning; monitor data/prediction drift (PSI/KS); run a shadow challenger; retrain on drift or performance drop. 

**Next Steps**  
Consider **uplift modelling**, near-real-time scoring around churn-intent events, and new features (usage patterns, ticket sentiment) to improve early warning. 

**Code / Repo**  
[Repository](https://github.com/Amro6625/Customer-Churn-Project)
