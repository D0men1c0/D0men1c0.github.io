---
title: "Gemma Model Benchmark Suite"
collection: portfolio
permalink: /portfolio/gemma-benchmark-suite
excerpt: "An open-source toolkit designed to democratize LLM analysis and benchmarking with deep customization and minimal compute requirements."
date: 2025-05-01
header:
  image: /images/benchmark_models.gif
  teaser: /images/benchmark_models.gif
repo_url: 'https://github.com/D0men1c0/Benchmark-Gemma-Models'
paper_url: 'https://medium.com/@domenicolacavalla8/customizable-llm-evaluation-benchmarking-gemma-and-beyond-with-benchmark-gemma-models-9dc6a5266be8'
---

## Goal
To democratize Large Language Model (LLM) analysis by providing an open-source evaluation toolkit that runs on accessible hardware, offering deep customization with minimal compute requirements.

## Key Features
- **Broad Evaluation Scope**: Run **4+** LLM families (Gemma, LLaMA 2, Phi-2) across **5+** standard tasks (MMLU+) and **15+** metrics, including BLEU, ROUGE, BERTScore, and Toxicity.
- **Extreme Customization**: The entire pipeline is configurable via **YAML** files. Users can easily integrate their own models, datasets, evaluation logic, and prompt templates.
- **Low-Resource Optimization**: Engineered to run efficiently on free-tier hardware (like Google Colab T4 GPUs) through techniques like **4-bit quantization** and batch-size tuning.
- **Interactive Dashboard**: Includes an interactive **Streamlit dashboard** for visual exploration, comparison of model performance, and analysis of results.
- **Robustness and Quality**: The framework is built with modular components, features Pydantic-validated configuration, and has a **73% Pytest coverage** to ensure reliability.

## Key Metrics & Impact
- **Performance on Free Hardware**: Achieves a **4-minute** benchmark run for **500 samples** using the Gemma-2B model in 4-bit mode on a single Colab T4 GPU.
- **Democratized Access**: Enables students, researchers, and practitioners without access to expensive hardware to conduct meaningful and complex LLM evaluations.
- **Community Adoption**: The toolkit has been featured in tutorials and demos as a prime example of accessible LLM experimentation.

## Tech Stack
- Python, PyTorch, TensorFlow, Transformers, Hugging Face, Scikit-learn, Streamlit