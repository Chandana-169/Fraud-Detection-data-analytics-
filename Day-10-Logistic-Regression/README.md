# Day 10 — Logistic Regression

## Objective
Build a probabilistic baseline fraud classifier and evaluate it across all four datasets.

## Notebook Work
Cell 23 trains Logistic Regression on the processed, SMOTE-balanced training data. Performance is evaluated with precision, recall, F1-score and PR-AUC.

Cell 24 searches validation thresholds rather than assuming 0.50. The selected validation thresholds were approximately **0.83 Credit, 0.89 Financial, 0.95 Synthetic, and 0.89 Orders**.

Final test F1 scores were approximately **0.784 Credit, 0.324 Financial, 0.786 Synthetic, and 0.900 Orders**. This showed that Logistic Regression worked strongly on Synthetic and Orders, but was weaker on Financial.

## Outcome
Logistic Regression became an important baseline and was ultimately selected as the final model for Synthetic and Orders.

## Notebook Reference
Cells 23–25