# Fine-tuning DistilBERT for Natural Language Inference

## 👥 Team Information

**Course:** Deep Learning  
**Institution:** Telkom University  

| Name | NIM |
| :--- | :--- |
| **Fasya Burhanis Syauqi** | 1103223054 |
| **Muhammad Muhammad Farhan** | 11032320187 |

---

## 🎯 Purpose

This repository contains the implementation of **Task 3: Natural Language Inference (NLI)**.

The objective is to fine-tune a pre-trained **DistilBERT** model to perform sentence pair classification. Given a *Premise* and a *Hypothesis*, the model determines the logical relationship between them.

## 🔍 Project Overview

### The Task: Sentence Pair Classification
We utilize the **MultiNLI (MNLI)** dataset from the GLUE benchmark. The task is to classify the relationship between two sentences into one of three categories.

### The Model: DistilBERT Base Uncased
* **Architecture:** Distilled version of BERT (Transformer Encoder).
* **Approach:** The input is formatted as `[CLS] Premise [SEP] Hypothesis [SEP]`. The model learns to predict the relationship based on the `[CLS]` embedding.

### The Dataset: MultiNLI (GLUE)
* **Input:** Pair of sentences (Premise and Hypothesis).
* **Output:** Logical relationship:
  * 0: Entailment (True)
  * 1: Neutral (Unrelated)
  * 2: Contradiction (False)

---

## 📊 Technical Approach

### Model Configuration
* **Base Model:** `distilbert-base-uncased`
* **Tokenizer:** DistilBertTokenizer
* **Framework:** PyTorch & Hugging Face Transformers

### Training Configuration
* **Batch Size:** 32
* **Learning Rate:** 2e-5
* **Epochs:** 3
* **Optimizer:** AdamW

### Results
The model achieved an accuracy of approximately **65.5%** on the matched validation set (trained on a data subset).
