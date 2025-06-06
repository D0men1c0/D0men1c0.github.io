---
title: "Baldness Classification Project"
collection: portfolio
permalink: /portfolio/baldness-classification
excerpt: "A deep learning project to classify different stages of baldness using CNNs and pre-trained models like ResNet50 and VGG16."
order: 5
date: 2024-04-10
repo_url: 'https://github.com/D0men1c0/Bald-Classification'
---

## Goal
To accurately classify different stages of baldness from images, providing a tool that could assist in the early detection and intervention for hair loss. The project tackles a 5-class classification problem: bald, normal, stage1, stage2, and stage3.

## Technical Approach
1.  **Dataset**: The project uses a dataset of ~2100 images from Roboflow Universe, split into 1500 for training, 300 for validation, and 300 for testing.
2.  **Preprocessing**: Images are resized to various dimensions (up to 100x100) and converted to grayscale using OpenCV to create a uniform dataset.
3.  **Model Development**: The project explored multiple CNN architectures in PyTorch, ranging from simple custom-built networks to complex, pre-trained models like **ResNet50** and **VGG16** for transfer learning.
4.  **Training & Evaluation**: Models were trained with a batch size of 32 and evaluated using a comprehensive set of metrics, including accuracy, precision, recall, F1 score, and AUC, with confusion matrices for error analysis.

## Key Metrics & Results
- **Performance Variance**: The project highlighted the challenge of working with limited and slightly imbalanced data.
- **Simple CNN**: Achieved high metrics on the training set (**0.9**), but overfitted, resulting in poor performance on the test set (**0.4**).
- **VGG16 Model**: Showed better generalization, achieving a **precision of 0.84** on the train, validation, and test sets, although other metrics were lower (~0.2), indicating the difficulty of the multi-class problem.

## Tech Stack
- Python, PyTorch, OpenCV, Scikit-learn, Roboflow