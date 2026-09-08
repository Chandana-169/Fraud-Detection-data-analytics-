# Day 08 — Data Splitting

## Objective
Create separate training, validation, and test sets while preserving the fraud/non-fraud ratio.

## Notebook Work
Cell 15 separates each dataset into features (`X`) and target (`y`). Cell 16 uses a **stratified train/validation/test split**, keeping class proportions consistent across the three partitions.

The workflow uses an 80/10/10 split. Validation data is used for model and threshold decisions, while the final test set is kept for final performance reporting.

## Outcome
Four datasets received reproducible stratified train/validation/test partitions, providing a clean evaluation structure for the supervised and anomaly-detection stages.

## Notebook Reference
Cells 15–16