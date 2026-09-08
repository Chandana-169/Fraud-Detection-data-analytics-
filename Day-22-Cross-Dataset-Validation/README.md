# Day 22 — Cross-Dataset Validation

## Notebook Status
The verified notebook does **not contain a dedicated cross-dataset validation experiment** that trains on one dataset and tests on another.

## What Is Actually Evaluated
The notebook evaluates four datasets independently through the same overall modeling framework: Credit, Financial, Synthetic, and Orders. Each dataset keeps its own schema, preprocessing pipeline, models, threshold, and final evaluation.

This is useful for comparing model behavior across datasets, but it is not equivalent to true transfer validation because the feature spaces are different.

## Result
No cross-dataset F1/PR-AUC table is claimed here because a dedicated cross-dataset experiment is not present in the notebook.

## Notebook Reference
Independent multi-dataset evaluation: Cells 14–69