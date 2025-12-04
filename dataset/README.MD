# 👹 The Grumpy Doctogres Challenge

Welcome aboard, engineer! You've been assigned to the **Iron-Guts Hospital**, a state-of-the-art medical facility specializing in tissue analysis and classification.

## 🎯 Mission Objective

Design a deep learning model that can classify diseased human tissue samples into their correct molecular subtypes. Success means better diagnostics and treatment planning for patients.

## 🧌 Molecular Subtype Classification

Your task is to analyze microscopic tissue morphology and predict the correct molecular subtype:

- **Luminal A** - The most common and typically more responsive to hormone therapy
- **Luminal B** - A more aggressive subtype with poorer prognosis
- **HER2(+)** - Characterized by HER2 gene amplification; requires targeted therapy
- **Triple Negative** - The most challenging; requires precision-based treatment approaches

## 📊 Dataset Overview

The dataset contains **2,366 images** of different sizes, each paired with a binary mask that identifies diseased tissue regions.

| File | Samples | Description |
|------|---------|-------------|
| `train_data/` | 1,412 | Image/mask pairs for model training |
| `test_data/` | 954 | Image/mask pairs for final evaluation (unlabeled) |
| `train_labels.csv` | - | Ground-truth molecular subtype labels |

### Example: Tissue Sample with Corresponding Mask

![Tissue Sample with Mask](./readme_img.png)

*Left: Microscopic tissue image labeled as "Triple Negative". Right: Binary mask highlighting diseased regions. The use of masks is optional but may improve classification performance.*

## ✅ Validation Strategy

No validation split is provided by default. You should create your own validation split from the training data for model evaluation and hyperparameter tuning.

## 🚀 Getting Started

1. Extract the dataset files
2. Load the training images and labels
3. Create a validation split (e.g., 80/20 or 70/30)
4. Develop and train your classification model
5. Evaluate on the validation set
6. Generate predictions on the test set

## 📈 Expected Outcomes

- Build a robust deep learning classifier for tissue subtype prediction
- Achieve high accuracy on the test set
- Document your methodology and results
- Submit predictions for evaluation

---

**Good luck, and may your models be ever accurate! 🧠⚙️**
