# Day 14 — SVM Model Comparison

## Objective
Evaluate Support Vector Machine classification against the other supervised fraud-detection models.

## Notebook Work
Cell 31 trains an RBF-kernel `SVC` with probability estimates enabled. It evaluates fraud detection on each processed dataset using precision, recall, F1-score and PR-AUC.

Validation F1 was approximately **0.800 Credit, 0.266 Financial, 0.588 Synthetic, and 0.851 Orders**.

## Outcome
SVM provided a useful comparison model, performing reasonably on Credit and Orders but remaining weaker on Financial. Final model selection was based on the complete supervised and hybrid comparison rather than SVM alone.

## Notebook Reference
Cell 31