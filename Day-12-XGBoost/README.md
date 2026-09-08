# Day 12 — XGBoost

## Objective
Train a gradient-boosted tree model and compare its fraud-detection performance with earlier classifiers.

## Notebook Work
Cell 28 trains `XGBClassifier` with 300 estimators, depth 6, learning rate 0.05, subsampling 0.8, and column subsampling 0.8. Cell 29 optimizes the classification threshold on validation data, and Cell 30 evaluates the selected threshold on the untouched test set.

Validation F1 was approximately **0.840 Credit, 0.222 Financial, 0.788 Synthetic, and 0.900 Orders**. Validation thresholds were approximately **0.54, 0.23, 0.47, and 0.42** respectively.

Test F1 was approximately **0.818 Credit, 0.371 Financial, 0.769 Synthetic, and 0.895 Orders**.

## Outcome
XGBoost was the strongest supervised candidate for Credit and Financial and later became the supervised component of the hybrid model.

## Notebook Reference
Cells 28–30