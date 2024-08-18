# Drug-Likeness Prediction Using Deep Neural Networks

## Overview

This project focuses on predicting the drug-likeness of chemical compounds using advanced deep learning models. The drug-likeness of a compound refers to the likelihood that it will exhibit pharmacological activity and can be developed into a viable drug. This prediction is crucial in the early stages of drug discovery to filter out compounds that are unlikely to be effective as drugs.

### Models Used
1. **GCN_attentivefp_SIDER**: A Graph Convolutional Network (GCN) combined with an attentive fingerprint layer, trained on the SIDER dataset to predict drug-likeness based on the molecular structure.
2. **ChemBERTa**: A transformer-based model that uses the ChemBERTa architecture, fine-tuned specifically for predicting drug-likeness.

### Motivation
The process of identifying drug-like compounds from chemical libraries is complex and resource-intensive. By leveraging machine learning, especially deep learning models like GCN and transformers, we can significantly improve the efficiency of this process.


## Introduction

A drug is a chemical substance or combination of substances that alleviates symptoms in patients without causing severe side effects. The aim of this project is to develop models that can predict whether a given chemical compound is drug-like, which is a critical step in the drug discovery process.

## Background

Traditional methods of drug-likeness prediction often relied on rule-based approaches. However, recent advancements in machine learning have enabled more accurate predictions through models that can learn complex patterns from large datasets.

### Previous Approaches
- **Rule-based Predictions**: Early methods used fixed rules (e.g., Lipinski's Rule of Five) to predict drug-likeness.
- **Machine Learning Models**: More recent approaches use machine learning models trained on large datasets of known compounds to predict drug-likeness.

## Methodology

This project utilizes the miDruglikeness approach, which combines two different deep learning models:

1. **GCN_attentivefp_SIDER**: This model uses a Graph Convolutional Network with an attentive fingerprint layer to analyze the molecular structure of compounds.
2. **ChemBERTa**: A transformer-based model, ChemBERTa, is fine-tuned for the specific task of drug-likeness prediction.

## Datasets

The primary dataset used in this project is:

- **ZINC15**: A large database of commercially available compounds for virtual screening.

The dataset is preprocessed and split into training and testing sets to evaluate the models.

## Evaluation

The models are evaluated based on their accuracy, precision, recall, F1-score, and ROC-AUC. These metrics provide a comprehensive understanding of the model's performance in predicting drug-likeness.

### GCN_attentivefp_SIDER
| Stage                      | AUC  | ACC  |
|------------------------------|------|------|
| In vivo ability               | 0.962| 0.928|
| IND ability                   | 0.876| 0.834|
| Market approvability ability  | 0.848| 0.805|


### ChemBERTa
| Ability                      | AUC  | ACC  |
|------------------------------|------|------|
| In vivo ability               | 0.879| 0.911|
| IND ability                   | 0.763| 0.807|
| Market approvability ability  | 0.740| 0.740|





 
