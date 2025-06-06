---
title: 'Examining the Evolution of Language Among Dark Web Users'
date: 2024-09-15
permalink: /posts/2024/09/gsoc-dark-web-article/
tags:
  - NLP
  - GSoC
  - Dark Web
  - BERT
  - Security
  - Computer Vision
---

This post provides an overview of my **Google Summer of Code 2024** research project with **HumanAI**, where I investigated how language and themes evolve within Dark Web communities.

The project's core challenge was to move beyond simple keyword tracking and understand the shifting semantic landscape of illicit forums. To achieve this, I developed a multi-modal analysis pipeline to process over **500,000 discussion points**.

The technical approach involved:
- Using **BERTopic** to perform deep semantic clustering on text, identifying and consolidating 170 granular topics into 5 core themes.
- Integrating **CLIP** and **Vision Transformer (ViT)** models to analyze the visual content (images) shared alongside text, adding another layer of context.
- Conducting a **temporal analysis** to map how the prevalence and sentiment of these topics changed over time, revealing key trends and shifts in community focus.

The result is a dynamic view of how criminal narratives are formed and evolve, providing valuable insights for cybersecurity and social science research.

[Read the full, in-depth article on Medium.com](https://medium.com/@domenicolacavalla8/examination-of-the-evolution-of-language-among-dark-web-users-67fd3397e0fb)