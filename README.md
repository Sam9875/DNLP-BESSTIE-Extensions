# Extending BESSTIE: Prompt-Based vs Fine-Tuned Models for Dialectal Sentiment and Sarcasm Classification

Final project for **Deep Natural Language Processing (DNLP) 2025–2026**  
Politecnico di Torino  

This repository contains the implementation and experimental results for our extensions of the BESSTIE benchmark (ACL 2025).

---

## 📌 Project Overview

We extend the BESSTIE benchmark in two complementary directions.

---

### 🔹 Extension 1: Prompt-Based vs Fine-Tuned Models

We systematically compare:

- Fine-tuned encoder models
- NLI-based zero-shot models
- Instruction / pseudo zero-shot prompting

Evaluation:

- Macro-F1 (primary metric)
- en-AU
- en-IN
- en-UK varieties

Additional analysis:

- Welch’s independent t-test
- Cohen’s *d* effect size
- Cross-variety robustness comparison

---

### 🔹 Extension 2: Sarcasm-Only Training Improvements

We focus on the Sarcasm–Reddit subset and explore:

- Class-balancing data augmentation
- Surface-level lexical perturbations
- Supervised Contrastive Learning (SupCon + Cross-Entropy)

We analyze:

- Macro-F1
- Macro-Precision
- Macro-Recall
- Accuracy
- Confusion matrices
- False positive / false negative trade-offs

---

## 📊 Dataset

We use the official BESSTIE dataset:

https://huggingface.co/datasets/unswnlporg/BESSTIE

For Extension 2, we filter:

- Task = `sarcasm`
- Source = `reddit`

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/DNLP-BESSTIE-Extensions.git
cd DNLP-BESSTIE-Extensions
