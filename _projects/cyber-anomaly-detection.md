---
title: "AI Cyber Anomaly Detection — Network Intrusion Detection Pipeline"
one_liner: "Built and evaluated an end-to-end intrusion detection pipeline, emphasizing reliable metrics and realistic model performance."
order: 1
featured: true
repo_url: "https://github.com/ReginaOfTech/cyber_anomaly_detection"
tags: ["Python", "Cybersecurity", "Anomaly Detection", "Responsible ML"]
highlights:
  - "Built a repeatable pipeline from raw UNSW-NB15 ingestion through preprocessing, modeling, and evaluation."
  - "Identified unrealistic evaluation results, diagnosed the root cause, and corrected the pipeline to produce credible metrics."
  - "Compared baseline and tree-based models to balance interpretability and detection performance."
---

### Tech
Python • pandas • scikit-learn • Logistic Regression • Random Forest • Isolation Forest • XGBoost • LightGBM

### Overview
A personal, non-commercial research project applying machine learning to anomaly detection in network traffic using the **UNSW-NB15** intrusion detection dataset. The project emphasizes evaluation rigor, documentation quality, and engineering judgment over raw benchmark performance.

### Context
Intrusion detection systems operate under extreme class imbalance and adversarial conditions. High accuracy alone is misleading, and shortcuts in evaluation can produce results that look strong but fail in realistic detection settings.

### Approach
- Implemented a structured workflow to load and standardize UNSW-NB15 data for repeatable experiments.
- Trained and compared baseline and tree-based models using validation-first tuning.
- Evaluated performance using precision, recall, F1, and PR-AUC to reflect operational tradeoffs.
- Diagnosed and corrected evaluation issues to ensure results reflected realistic model behavior.

### Why this matters
This project demonstrates security-minded ML engineering: skepticism toward “perfect” results, disciplined evaluation practices, and pipelines designed to support trustworthy decision-making.

### Links
- [GitHub](https://github.com/ReginaOfTech/cyber_anomaly_detection)
