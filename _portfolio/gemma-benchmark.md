---
title: "Gemma Model Benchmark Suite"
collection: portfolio
permalink: /portfolio/gemma-benchmark-suite
excerpt: "An open-source toolkit designed to democratize LLM analysis and benchmarking, with deep customization and minimal compute requirements."
date: 2025-05-29
header:
  image: /assets/benchmark_models.gif
  teaser: /assets/benchmark_models.gif
repo_url: 'https://github.com/D0men1c0/Benchmark-Gemma-Models'
paper_url: 'https://medium.com/@domenicolacavalla8/customizable-llm-evaluation-benchmarking-gemma-and-beyond-with-benchmark-gemma-models-9dc6a5266be8'
---

## Goal
This project democratizes Large Language Model (LLM) evaluation, enabling researchers, students, and practitioners to run meaningful benchmarks on their own data and terms, even on free-tier GPUs like Google Colab T4.

## What It Does
GemmaModel is an open-source evaluation toolkit built with YAML-first configurability and modular components. It allows users to:
- Run **4+** LLM families across **5+** tasks and **15+** metrics (BLEU, ROUGE, BERTScore, Toxicity, etc.).
- Integrate their own models, datasets, prompts, and evaluation logic.
- Plug in custom handlers, metrics, scripts, and templates for full extensibility.
- Visualize results and insights through an interactive Streamlit dashboard.

## Impact
- **Accessibility**: Enables meaningful evaluation of LLMs on free-tier GPUs.
- **Performance**: Achieves **4-minute** benchmarking for **500 samples** using Gemma-2B in **4-bit** mode, thanks to optimizations like quantization and batch-size tuning.
- **Adoption**: Used to evaluate and compare models like Gemma, LLaMA 2, and Phi-2 in tutorials and demos showcasing accessible LLM experimentation.

> “LLM evaluation for the rest of us” — open, flexible, and built to scale from personal research to comparative pipelines.