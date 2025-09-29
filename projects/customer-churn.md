---
layout: single
title: "Customer Churn Prediction"
permalink: /projects/customer-churn/
---


**Problem**  
Predict which customers are likely to churn next cycle so retention can intervene early (cost-sensitive framing prioritising recall on churn while controlling precision to protect ROI). :contentReference[oaicite:0]{index=0}

**Data & Preparation**  
Demographics, subscribed services, contract type, payment method, tenure, billing. Cleaning, missing-value treatment, categorical encoding, selective scaling, and a leakage-safe train/validation/test split. :contentReference[oaicite:1]{index=1}

**EDA Highlights (what drives churn)**  
- Highest churn: **month-to-month** contracts, **short tenure**, and **electronic check** payments.  
- Higher monthly charges and certain service bundles elevate churn risk.  
- Interaction effects (e.g., **contract × tenure**) are important → tree models capture these without manual crosses. :contentReference[oaicite:2]{index=2}

**Modelling Strategy & Rationale**  
Benchmarked Logistic Regression and tree ensembles; **XGBoost** chosen for best AUC–Recall balance, non-linear interactions, and strong tabular performance. Calibrated probabilities and set an operating threshold aligned to business costs. :contentReference[oaicite:3]{index=3}

**Results (hold-out test)**  
- **AUC = 0.841**, **F1 = 0.637**.  
- Key drivers (consistent across explainability views): **tenure, contract type, payment method, monthly charges**. :contentReference[oaicite:4]{index=4}

**Business Impact**  
Risk scores feed CRM; prioritise top deciles first; A/B test to quantify uplift and refine thresholds/offers by micro-segment. :contentReference[oaicite:5]{index=5}

**Deployment & Monitoring**  
Batch scoring (daily/weekly) with versioning; monitor data/prediction drift (PSI/KS); run a shadow challenger; retrain on drift or performance drop. :contentReference[oaicite:6]{index=6}

**Next Steps**  
Consider **uplift modelling**, near-real-time scoring around churn-intent events, and new features (usage patterns, ticket sentiment) to improve early warning. :contentReference[oaicite:7]{index=7}

**Code / Repo**  
[Repository](https://github.com/Amro6625/Customer-Churn-Project)
