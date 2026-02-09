---
title: 'Text2Motion: From Text to 3D Animation for Any Mesh'
date: 2025-10-15
permalink: /posts/2025/10/text2motion-article/
tags:
  - 3D Animation
  - Deep Learning
  - PyTorch
  - Transformers
  - Computer Vision
---

This post introduces **Text2Motion**, a three-stage pipeline that automates the full 3D character animation workflow — from static meshes to text-aligned motion sequences.

The project tackles three core challenges: automatic rigging and skinning using PointNet++, text-conditioned motion generation via a topology-aware transformer diffusion model with SBERT and T5 encodings, and training with Geodesic + InfoNCE losses for topologically consistent and semantically aligned results.

The system achieved 92% armature classification accuracy on the Truebones Zoo dataset, demonstrating that end-to-end text-driven animation of arbitrary meshes is feasible.

[Read the full article on Medium.com](https://medium.com/@domenicolacavalla8/text2motion-from-text-to-3d-animation-for-any-mesh-5f437165eb96)
