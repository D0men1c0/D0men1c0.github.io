---
title: "Text2Motion"
collection: portfolio
permalink: /portfolio/text2motion
excerpt: "A three-stage pipeline automating 3D animation from static meshes to text-aligned motion using PointNet++, transformer diffusion, and SBERT/T5 encodings."
order: 2
date: 2025-10-15
repo_url: 'https://github.com/D0men1c0/Text2Motion'
---

## Goal
To develop an end-to-end pipeline that automates 3D character animation, taking static meshes and generating text-aligned motion sequences through automatic rigging, skinning, and motion synthesis.

## Technical Approach
The system is organized in three stages:

1. **Automatic Rigging & Skinning**: A **PointNet++** model predicts joint positions and skinning weights directly from 3D mesh geometry, eliminating the need for manual rigging.
2. **Text-Conditioned Motion Generation**: A **topology-aware transformer diffusion model** generates motion sequences conditioned on natural language descriptions, using **SBERT** and **T5** text encodings.
3. **Loss & Training**: The model is trained with a combination of **Geodesic loss** and **InfoNCE** contrastive loss to ensure topologically consistent and semantically aligned motion.

## Key Metrics & Results
- Achieved **92% armature classification accuracy** on the Truebones Zoo dataset.
- The pipeline successfully automates the full workflow from static mesh to animated character driven by text descriptions.
- Published results in the "Text2Motion" article.

## Tech Stack
- Python, PyTorch, Transformers, CUDA, OpenCV, SBERT, T5
