# Day 21 — Model Calibration

## Notebook Status
A separate, completed calibration experiment is **not present as a dedicated cell** in the verified notebook sequence.

## What the Notebook Does Instead
The project explicitly produces probability scores and performs validation-based threshold optimization. Final evaluation uses precision, recall, F1-score and PR-AUC, and the deployment package stores the chosen decision threshold with the selected model.

## Result
No calibration curve, Brier score, isotonic calibration, Platt scaling, or calibrated-model result is claimed because those operations are not present in the notebook source.

## Notebook Reference
Probability and threshold workflow: Cells 23–30 and final model configuration in Cells 56–69