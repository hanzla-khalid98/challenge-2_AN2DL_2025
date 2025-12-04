# 👹 Artificial Neural Networks & Deep Learning - Challenge 2

**Second Challenge** of the Artificial Neural Networks and Deep Learning course (A.Y. 2025-2026)

## 🎯 Objective

Classify human tissue samples into their correct **molecular subtypes** using deep learning. Each image is from a low-magnification Whole Slide Image (WSI) of tissue, and your task is to assign each to one of four disease subtypes.

## 🧌 Molecular Subtypes

Your classification targets are:

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

![Tissue Sample with Mask](dataset/readme_img.png)

*Left: Microscopic tissue image labeled as "Triple Negative". Right: Binary mask highlighting diseased regions. The use of masks is optional but may improve classification performance.*

## ⏰ Timeline

- **Start:** A day ago
- **Deadline:** December 13, 23:59
- **Time remaining:** 9 days

## 📋 How to Participate

### 1. Registration

- Register via the Google form (Kaggle account must be linked to institutional email: `name.surname@mail.polimi.it`)
- Your Kaggle display nickname must match the form
- Apply to the competition

### 2. Team Formation

- **Mandatory:** Create or join a team in the 'Team' tab
- **Team size:** 3-4 members
- Looking for teammates? Wait 24-48 hours after form deadline for group assignments

### 3. Submit Solution

- Submit a `.csv` file with predictions
- Format: `sample_index,label` (one row per test image)
- **Deadline:** December 13, 23:59

## 📤 Submission Format

Your submission file must be a CSV with the following structure:

```
sample_index,label
img_0000.png,HER2(+)
img_0001.png,Luminal B
img_0002.png,Luminal A
...
```

## 🥇 Evaluation

Your models will be evaluated on the **F1-Score** (macro-averaged across all classes).

### Leaderboard Metrics

$$F1 = \frac{2 \times \text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}} = \frac{TP}{TP + \frac{1}{2}(FP + FN)}$$

Where:
- **TP** = True Positives
- **FP** = False Positives
- **FN** = False Negatives

### Scoring

- **Leaderboard Score** + **Report Score** = **0-5 points** (added to written exam grade)
- **Bonus:** +0.5 additional points for exceptional works

### Important Notes

- During the competition, submissions are evaluated on a **public test subset**
- Final results on a **separate private test subset** will be released on December 13, 23:59
- No validation split is provided—create your own (e.g., 70/30 or 80/20)

## 📄 Final Report Requirements

**Due:** December 13, 23:59

Submit a **PDF report (max 3 pages + references)** using the [Latex Template on Overleaf](https://www.overleaf.com/) that includes:

1. Team member information
2. Model development process
3. Ideas behind your final solution
4. All necessary details to demonstrate your work

**Submission:** Email to `airlab.official.polimi@gmail.com`

### Attachments Required

1. **PDF Report** - Your final report
2. **ZIP File** - Containing one or more fully-executed Jupyter notebooks with:
   - Code for creating and training models
   - Local performance results (visible in output cells)
   - Well-commented and reproducible code
   - Clear documentation of functions, variables, and main steps

**⚠️ All files must be attached directly—no links. Emails not following the specified format will not be considered.**

## 📧 Email Format (Required)

**Subject:** `AN2DL25 - Challenge 2`

**Body:**

```
GROUP_NAME: [Your group name]

STUDENT_1_NAME: [Name Surname]
STUDENT_1_ID: [matricola]
STUDENT_1_EMAIL: [email]

STUDENT_2_NAME: [Name Surname]
STUDENT_2_ID: [matricola]
STUDENT_2_EMAIL: [email]

STUDENT_3_NAME: [Name Surname]
STUDENT_3_ID: [matricola]
STUDENT_3_EMAIL: [email]

STUDENT_4_NAME: [Name Surname] (if applicable)
STUDENT_4_ID: [matricola] (if applicable)
STUDENT_4_EMAIL: [email] (if applicable)

REPORT_FILENAME: [Your report filename .pdf]
ZIP_FILENAME: [Your zip filename .zip]
```

## 🚀 Getting Started

1. Extract the dataset files
2. Load training images and labels
3. Create a validation split for local evaluation
4. Develop and train your classification model
5. Evaluate on the validation set and optimize
6. Generate predictions on the test set
7. Prepare your report and notebooks
8. Submit before the deadline

---

**Good luck, and may your models be ever accurate! 🧠⚙️**
