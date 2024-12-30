# Deep Learning for NLP - Attention Mechanisms

This repository contains the implementation of Exercise 04 for the **Deep Learning for NLP** course. The assignment explores transformer-based models, focusing on visualizing attention mechanisms and evaluating decoding strategies. This work adheres strictly to the guidelines and provided templates by the instructors.

## Project Overview

The assignment consists of two main tasks:

### Task 1: Visualizing Attention Mechanisms

- **Objective**: Analyze the attention maps of randomly initialized BERT, pretrained BERT, and GPT-2 models.
- **Instructor Contributions**: Provided guidance on model initialization, tokenization, and visualization frameworks.
- **Student Contributions**:
  - Implemented scripts for processing token sequences and extracting attention outputs.
  - Visualized attention maps using `bertviz`'s `model_view` and `head_view`.
  - Compared hierarchical patterns, redundancy, and interpretability between BERT and GPT-2 models.

### Task 2: Decoding Strategies

- **Objective**: Compare multiple decoding algorithms on the same model and prompt to analyze their impact on text quality.
- **Instructor Contributions**: Provided sample prompts and basic decoding setups.
- **Student Contributions**:
  - Extended the decoding analysis by implementing and evaluating additional strategies.
  - Quantified differences in generated text based on entropy and other metrics.

## Repository Structure

- **Instructor Setup**:
  - Baseline configurations for models and datasets.
  - Scripts for ensuring compliance with exercise guidelines.

- **Student Additions**:
  - Extensions to model analysis.
  - Custom visualizations and entropy-based evaluations.
  - Detailed observations and interpretations for each task.

## Observations and Insights

### Task 1: Attention Mechanisms

- **Randomly Initialized BERT**: Exhibits uniform attention patterns across tokens.
- **Pretrained BERT**: Captures complex relationships and attends to global structures in higher layers.
- **GPT-2**: Focuses on causal dependencies, with heads specializing in syntactic or positional relationships.

### Task 2: Decoding Strategies

- **Entropy Analysis**: Demonstrates how certain heads exhibit high entropy, capturing broader contexts, while others focus narrowly.
- **Decoding Comparisons**: Highlights the trade-offs between text diversity and coherence using various algorithms.

## Key Visualizations

- Attention heatmaps for BERT and GPT-2 models.
- Entropy trends across layers and heads, visualized interactively using Plotly.
- Comparative plots of decoding outputs.

## Guidelines and Compliance

This work strictly follows the instructor's directives, including:

- Using the provided imports and frameworks.
- Maintaining compatibility with the environment file.
- Adhering to naming conventions and submission formats.

## Requirements
- matplotlib==3.7.1
- nltk==3.8.1
- pandas==1.5.3
- scikit-learn==1.2.2
- scipy==1.10.1
- seaborn==0.12.2
- spacy==3.6.1
- datasets==3.0.1
- torch==2.0.1
- torchtext==0.15.2
- transformers==4.24.0
- evaluate==0.4.0
- rouge-score==0.1.2
- py7zr
- bertviz
- plotly>=5.0.0

