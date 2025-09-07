---
layout: home
author_profile: true
title: "Data Science Portfolio"
excerpt: "End-to-end ML and NLP projects with measurable business impact."
header:
  overlay_color: "#000"
  overlay_filter: "0.35"
  overlay_image: /Amro_Portfolio/assets/images/hero.jpg
intro: |
  **Hi, I'm Amro.** UK-based Data Scientist (MSc AI & Data Science, University of Hull). I design, build, and deploy practical ML/NLP solutions that reduce risk, lift conversions, and improve operations.
feature_row:
  - image_path: /Amro_Portfolio/assets/images/social-media.png
    alt: "Sentiment and Risk Detection"
    title: "Sentiment and Risk Detection (Humberside F&R)"
    excerpt: "Up to 94% validation accuracy; faster incident prioritisation."
    url: "/Amro_Portfolio/projects/social-media/"
    btn_label: "View case study"
    btn_class: "btn--primary"
  - image_path: /Amro_Portfolio/assets/images/landmark.png
    alt: "Landmark Classification"
    title: "Landmark Detection — Image Classification"
    excerpt: "~98% test accuracy with ResNet on curated dataset."
    url: "/Amro_Portfolio/projects/landmark-detection/"
    btn_label: "View case study"
    btn_class: "btn--primary"
  - image_path: /Amro_Portfolio/assets/images/uk-accidents.png
    alt: "UK Accident Analysis"
    title: "UK Road Traffic Accident Analysis"
    excerpt: "Patterns & drivers of severity; stacking classifier for prediction."
    url: "/Amro_Portfolio/projects/uk-accidents/"
    btn_label: "View case study"
    btn_class: "btn--primary"
---

{% if page.intro %}
<div class="notice--primary">{{ page.intro | markdownify }}</div>
{% endif %}

{% include feature_row %}