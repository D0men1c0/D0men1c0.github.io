---
title: "Knowledge Injection XAI"
collection: portfolio
permalink: /portfolio/knowledge-injection-xai
excerpt: "A distributed framework predicting out-of-distribution robustness using only XAI metrics from clean data, integrating DINOv2, LoRA, and XGBoost."
order: 1
date: 2026-01-15
repo_url: 'https://github.com/D0men1c0/Knowledge-Injection-XAI'
---

## Goal
To develop a distributed framework that can predict out-of-distribution (OOD) robustness of models using only Explainable AI (XAI) metrics extracted from clean data, eliminating the need for corrupted test sets during evaluation.

## Technical Approach
- Built a **Spark pipeline** integrating **DINOv2** as the backbone vision encoder with **LoRA** (Low-Rank Adaptation) fine-tuning and **XGBoost** for robustness forecasting.
- Extracted XAI metrics from clean data to predict how models would perform under distribution shifts and corruptions.
- Compared low-rank vs. high-rank adapter configurations to analyze their impact on corruption resistance.

## Key Metrics & Results
- Achieved **0.739 ROC-AUC** on the OOD robustness prediction task.
- Demonstrated that **low-rank adapters resist corruptions 19% better** than high-rank ones, providing actionable insights for model design.
- The distributed Spark pipeline enables scalable evaluation across large model collections.

## Tech Stack
- Python, PyTorch, Apache Spark, DINOv2, LoRA, XGBoost
