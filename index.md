---
layout: home
author_profile: true
title: "Data Science Portfolio"
excerpt: "End-to-end ML and NLP projects with measurable business impact."
header:
  overlay_color: "#000"
  overlay_filter: "0.35"
  overlay_image: {{ site.baseurl }}/assets/images/hero.jpg
intro: |
  **Hi, I'm Amro.** A UK-based Data Scientist with an MSc in AI and Data Science (University of Hull).
  I design, build, and deploy practical ML/NLP solutions that reduce risk, lift conversions, and improve operations.
  I am comfortable across the lifecycle: data collection, feature engineering, model development, evaluation, and deployment.
feature_row:
  - image_path: {{ site.baseurl }}/assets/images/social-media.png
    alt: "Sentiment and Risk Detection"
    title: "Sentiment and Risk Detection (Humberside F&R)"
    excerpt: "Up to 94% validation accuracy; faster incident prioritisation."
    url: "{{ site.baseurl }}/projects/social-media/"
    btn_label: "View case study"
    btn_class: "btn--primary"
  - image_path: {{ site.baseurl }}/assets/images/credit-risk.png
    alt: "Credit Risk"
    title: "Credit Risk - Default Prediction"
    excerpt: "AUC-ROC 0.85, 78% accuracy; ~10% fewer false negatives."
    url: "{{ site.baseurl }}/projects/credit-risk/"
    btn_label: "View case study"
    btn_class: "btn--primary"
  - image_path: {{ site.baseurl }}/assets/images/recsys.png
    alt: "Recsys"
    title: "Recommendation System"
    excerpt: "+30% retrieval accuracy; +20% conversions; -40% latency."
    url: "{{ site.baseurl }}/projects/recsys/"
    btn_label: "View case study"
    btn_class: "btn--primary"
---

{% if page.intro %}
<div class="notice--primary">{{ page.intro | markdownify }}</div>
{% endif %}

{% include feature_row %}