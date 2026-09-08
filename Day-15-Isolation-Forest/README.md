# Day 15 — Isolation Forest

## Objective
Add unsupervised anomaly detection to identify transactions that look unusual without directly training on fraud labels.

## Notebook Work
Cell 36 trains an `IsolationForest` with 300 trees and contamination set to 0.04. The anomaly predictions are evaluated against the fraud labels for comparison purposes.

Validation F1 scores were approximately **0.561 Credit, 0.049 Financial, 0.532 Synthetic, and 0.254 Orders**.

## Outcome
Isolation Forest alone was weaker than the supervised models, especially on Financial. Its anomaly score was nevertheless useful later as a complementary signal in the hybrid fraud-risk model.

## Notebook Reference
Cell 36