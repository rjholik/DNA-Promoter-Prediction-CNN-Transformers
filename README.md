# Deep Learning Models for Promoter Prediction

## Overview

This project explores deep learning approaches for promoter prediction from DNA sequences, with a focus on comparing convolutional neural networks (CNNs) and transformer-based models.

The goal is to understand how different architectures capture sequence patterns and to evaluate their performance on genomic data.

---

## Project Structure

data/
├── raw/ # original datasets (not tracked by git)
├── processed/ # cleaned datasets

notebooks/
├── 00_data_setup.ipynb
├── 01_data_exploration.ipynb
├── 02_preprocessing.ipynb
└── 03_model_training.ipynb

src/ # (in progress) reusable code

---

## Current Progress

- Data pipeline setup
- Genome loading and validation
- Exploratory data analysis:
  - base composition
  - GC content
  - k-mer frequency analysis

🚧 Model development in progress

---

## Methods

### Data
- Human genome (GRCh38, chromosome 1)
- Promoter dataset (UCI)

### Analysis
- Base composition
- GC content
- K-mer frequency

### Models (planned)
- Convolutional Neural Networks (CNNs)
- Transformer-based models

---

## Results (so far)

- GC content ~38.6% (consistent with human genome)
- Balanced nucleotide distribution (A≈T, C≈G)
- Presence of genomic gaps (N regions)

---

## Future Work

- Sequence preprocessing pipeline
- Model implementation (CNN, Transformer)
- Performance comparison
- Model interpretation (saliency, attention)

---

## Requirements

```bash
pip install numpy pandas matplotlib seaborn torch

Notes
Large genome files are excluded via .gitignore
Notebooks are organized as a step-by-step pipeline
Author

Radek Holik