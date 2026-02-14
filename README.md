# DNLP-BESSTIE-Extensions
BESSTIE: A Benchmark for Sentiment and Sarcasm Classification for Varieties of English
# Extending BESSTIE: Prompt-Based vs Fine-Tuned Models for Dialectal Sentiment and Sarcasm Classification

This repository contains the implementation and experiments for the DNLP 2025–2026 final project at Politecnico di Torino.

## 📌 Project Overview

We extend the BESSTIE benchmark (ACL 2025) in two directions:

### Extension 1: Prompt-Based vs Fine-Tuned Models
We compare:
- Fine-tuned encoder models
- NLI-based zero-shot models
- Instruction/pseudo zero-shot prompting

We evaluate macro-F1 across:
- en-AU
- en-IN
- en-UK

We also perform:
- Welch’s t-test
- Cohen’s d effect size analysis

---

### Extension 2: Sarcasm-Only Training Improvements

We focus on the Sarcasm-Reddit subset and explore:

- Class-balancing data augmentation
- Surface-level lexical perturbations
- Supervised Contrastive Learning (SupCon + CE)

We analyze:
- Macro-F1
- Precision / Recall
- Confusion matrices
- Error trade-offs

---

## 📊 Dataset

We use the BESSTIE dataset:

https://huggingface.co/datasets/unswnlporg/BESSTIE

Sarcasm-only experiments filter:
- Task = Sarcasm
- Source = Reddit

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/DNLP-BESSTIE-Extensions.git
cd DNLP-BESSTIE-Extensions
