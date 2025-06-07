---
title: "AquaAware: A Two-Phase Learning System for Water Conservation"
collection: portfolio
date: 2024-04-01
excerpt: "A smart water-saving system that uses a two-phase machine learning approach to train users and optimize household water consumption."
repo_url: 'https://github.com/D0men1c0/AquaAware'
---

AquaAware is a project designed to reduce water consumption in homes by providing real-time recommendations for various tasks like brushing teeth, washing hands, showering, and washing dishes. The system employs a two-phase machine learning algorithm to first train users on best practices and then further optimize their personal habits.

### Phase 1: Supervised Learning for Best Practices

Initially, the system uses a dataset containing optimal water consumption levels and time durations for common household tasks.

* **Algorithm:** A **Decision Tree** classifier is trained on this "best practice" data.
* **Functionality:** As the user consumes water, the device records the usage and time. The Decision Tree predicts the ongoing task and provides real-time recommendations to help the user align their habits with water-saving standards.
* **Goal:** The primary objective of this phase is to guide the user towards adopting more sustainable habits and reducing initial water wastage.

### Phase 2: Unsupervised Learning for Personalized Optimization

Once the user has consistently adopted the recommended best practices, the system transitions to a personalized optimization phase.

* **Data Collection:** The system begins to store the user's new, more efficient water usage patterns in a new dataset, but without task labels.
* **Unsupervised Learning:** Since the device cannot automatically classify these new patterns, the **K-Means** clustering algorithm is used. Knowing the number of tasks beforehand, K-Means groups the unlabeled data into distinct clusters, effectively re-identifying the tasks based on the user's unique behavior.
* **Retraining:** Once the new data is labeled through clustering, a new **Decision Tree** model is trained on this personalized dataset.
* **Goal:** This second model provides even more refined predictions and recommendations, pushing the user to consume only what is strictly necessary, thereby minimizing waste beyond the standard best practices.

### Design Choices

* **Decision Tree** was selected as the supervised learning algorithm due to its high accuracy and significantly faster response times compared to alternatives like K-Nearest Neighbors (KNN).
* **K-Means** was chosen for the unsupervised learning task because the number of clusters (i.e., the number of distinct household tasks) was known in advance, making it a highly efficient choice.