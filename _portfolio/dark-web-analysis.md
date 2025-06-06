---
title: "Dark Web Topic Analysis (GSoC @ HumanAI)"
collection: portfolio
permalink: /portfolio/dark-web-analysis
excerpt: "A project focused on uncovering how language tied to criminal behavior evolves over time within Dark Web forums."
date: 2024-09-30
header:
  image: gsoc.png
  teaser: gsoc.png
repo_url: 'https://github.com/humanai-foundation/ISSR/tree/main/ISSR_Dark_Web_Domenico_Lacavalla'
paper_url: 'https://medium.com/@domenicolacavalla8/examination-of-the-evolution-of-language-among-dark-web-users-67fd3397e0fb'
---

## Goal
This project, developed for Google Summer of Code at HumanAI, focuses on uncovering how language tied to criminal behavior evolves over time within Dark Web forums, providing insights for security and linguistic research.

## Technical Approach
- Analyzed over **500,000 discussion points** from underground marketplaces and illicit forums.
- Used **BERT** and **BERTopic** for semantic embedding and clustering to identify emerging criminal themes.
- Integrated **CLIP** and **ViT** to examine visual content alongside textual data, creating a multi-modal analysis pipeline.
- Conducted **temporal analysis** to track linguistic shifts and the evolution of topics across months and years.

## Impact
- **Identified Key Themes**: Extracted 5 core topic categories, creating a temporal view of how narratives and terminology changed.
- **Predictive Modeling**: Deployed predictive models on Hugging Face to forecast thematic evolution.
- **Open Science**: The results, models, and code were communicated through an in-depth [Medium article](https://medium.com/@domenicolacavalla8/examination-of-the-evolution-of-language-among-dark-web-users-67fd3397e0fb) and fully open-sourced on GitHub.