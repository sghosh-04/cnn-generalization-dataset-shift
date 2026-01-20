# On the Generalization of CNN-Based AI-Generated Image Detectors Under Dataset Shift

This repository contains the code and experiments for an independent research project
studying the robustness and generalization of CNN-based AI-generated image detectors
under dataset shift.

## 🔍 Problem Statement
CNN-based detectors for AI-generated images often achieve high accuracy on curated
benchmark datasets. However, their reliability under real-world distributional
variations remains poorly understood.

This work investigates how dataset shift impacts the performance and failure modes
of commonly used CNN architectures.

## 🧠 Research Questions
- How well do CNN-based AI-generated image detectors generalize from synthetic
  training datasets to real-world image distributions?
- What failure patterns emerge under out-of-distribution evaluation?

## 🧪 Methodology
- Models: EfficientNet, ResNet50 (transfer learning)
- Task: Binary classification (real vs AI-generated images)
- Evaluation:
  - In-distribution vs out-of-distribution testing
  - Confusion matrices, ROC curves
  - Grad-CAM visualizations for failure analysis

## 📊 Key Findings
- Models achieve strong in-distribution accuracy on curated datasets.
- Significant performance degradation is observed under dataset shift.
- Failure analysis reveals reliance on low-level texture artifacts rather than
  robust semantic cues.

## 📁 Repository Structure
- `paper/` – Full technical report (PDF)
- `experiments/` – Training and evaluation scripts
- `notebooks/` – Analysis and visualization
- `figures/` – Confusion matrices, ROC curves, Grad-CAM examples

## 📄 Paper
The full report is available here:
[`paper/paper.pdf`](paper/paper.pdf)

## 🚀 Reproducibility
Install dependencies:
```bash
pip install -r requirements.txt
