# Deep Learning Models for Promoter Prediction

🚧 Work in progress — building deep learning models (CNNs and Transformers) for promoter prediction from genomic DNA sequences.

---

## Overview

This project explores deep learning approaches for promoter prediction from DNA sequences, with a focus on comparing convolutional neural networks (CNNs) and transformer-based architectures.

The goal is to understand how different models capture sequence patterns and to evaluate their performance on genomic data.

---

## Project Structure

    data/
    ├── raw/        # original datasets (not tracked by git)
    ├── processed/  # cleaned datasets

    notebooks/
    ├── 00_data_setup.ipynb
    ├── 01_data_exploration.ipynb
    ├── 02_preprocessing.ipynb
    └── 03_model_experiments.ipynb

    src/            # (in progress) reusable code

---

## Data

The datasets are not included in this repository due to their size.

### Genome
Human genome (GRCh38, chromosome 1):  
https://ftp.ensembl.org/pub/release-110/fasta/homo_sapiens/dna/

### Promoter Dataset
UCI Molecular Biology (Promoter Gene Sequences):  
https://archive.ics.uci.edu/

After downloading, place files into:

    data/raw/genome/
    data/raw/uci_promoter/

---

## Current Progress

- Data pipeline setup
- Genome loading and validation
- Exploratory data analysis:
  - Base composition
  - GC content (~38.6%)
  - K-mer frequency analysis

---

## Methods

### Data Processing
- FASTA parsing
- Filtering ambiguous bases (N)
- Sequence sampling

### Analysis
- Base composition
- GC content (global and local)
- K-mer frequency analysis

### Models (planned)
- Convolutional Neural Networks (CNNs)
- Transformer-based models

---

## Example Analysis

*(Add figures here later)*

---

## Future Work

- Sequence preprocessing pipeline
- Model implementation (CNN, Transformer)
- Performance evaluation
- Model interpretation (e.g., saliency maps, attention)

---

## Requirements

    pip install numpy pandas matplotlib seaborn torch

---

## Notes

- Large genome files are excluded via `.gitignore`
- Notebooks are organized as a step-by-step pipeline

---

## Author

Radek Holik  
M.S. in Artificial Intelligence  
Renal Research Institute, Fresenius Medical Care