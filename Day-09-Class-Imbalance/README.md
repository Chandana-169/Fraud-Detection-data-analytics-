# Day 09 — Class Imbalance

## Objective
Handle the minority fraud class so models do not simply favor normal transactions.

## Notebook Work
The datasets contain only 4% fraud, making class imbalance an important modeling issue. Cell 19 applies **SMOTE only to the training data**, after preprocessing. Validation and test data are not oversampled.

The Credit dataset receives a corrected preprocessing pass after `MerchantID` is recognized as categorical, followed by a fresh SMOTE application in Cells 20–22.

## Outcome
Training data is balanced using synthetic minority oversampling while validation/test distributions remain untouched. This supports fair evaluation with precision, recall, F1, and PR-AUC rather than accuracy alone.

## Notebook Reference
Cells 19–22