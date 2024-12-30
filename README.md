# DL for NLP - Attention Mechanisms

This repository contains the implementation of **Exercise 04** for the "Deep Learning for NLP" course. The exercise focuses on implementing various attention mechanisms for NLP tasks, including Bahdanau and Luong attention models, within sequence-to-sequence frameworks. The task explores alignment-based techniques to improve sequence modeling.

## Overview

The project includes the following:
1. **Bahdanau Attention Mechanism**:
   - Implements additive attention.
   - Evaluates its impact on sequence-to-sequence translation tasks.
2. **Luong Attention Mechanism**:
   - Implements dot-product attention.
   - Comparison of its effectiveness against Bahdanau attention.
3. **Custom Seq2Seq Architecture**:
   - Encoder-decoder architecture with GRU-based RNNs.
   - Attention module integrated into the decoder for context vector calculation.

This repository adheres to the course submission guidelines and retains the original structure provided by the instructors.

## My Contributions

The provided structure included the high-level task description and some starter code. My key contributions include:
- Implementation of the Bahdanau and Luong attention mechanisms.
- Integration of attention modules into the Seq2Seq architecture.
- Custom training loop with early stopping to prevent overfitting.
- Model evaluation using BLEU scores for translation quality assessment.

## Key Features

### Bahdanau Attention
- Additive attention mechanism designed to compute alignment scores.
- Context vector calculated as a weighted sum of encoder outputs.
- Allows the decoder to focus on relevant parts of the input sequence.

### Luong Attention
- Dot-product attention mechanism that simplifies alignment computation.
- General attention variant used to compute context vectors.
- Enhanced computational efficiency compared to additive attention.

### Seq2Seq Architecture
- **Encoder**: GRU-based RNN processes input sequences into hidden states.
- **Decoder**: GRU-based RNN uses context vectors from attention mechanisms for decoding.
- **Attention Mechanisms**: Integrated into the decoder for context-aware predictions.

### Training and Evaluation
- Custom training loop implemented with:
  - Cross-entropy loss.
  - Optimizer: Adam with a learning rate scheduler.
- Evaluation metrics:
  - BLEU scores to assess translation quality.
  - Per-sequence alignment analysis to visualize attention weights.

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

