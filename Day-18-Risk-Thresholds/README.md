# Day 18 — Risk Thresholds

## Objective
Choose fraud-decision thresholds from validation data instead of relying on the default 0.50 probability cutoff.

## Notebook Work
Cells 24 and 29 optimize supervised thresholds using validation F1. Cells 47 and 54 perform the equivalent threshold search for the hybrid risk scores, including the corrected production-safe hybrid score.

Final selected thresholds were approximately:
- Credit Hybrid: **0.52**
- Financial Hybrid: **0.27**
- Synthetic Logistic Regression: **0.95**
- Orders Logistic Regression: **0.89**

These thresholds are then applied to the untouched test data for final reporting.

## Outcome
Threshold selection is separated from final testing, allowing the project to trade off precision and recall according to the fraud-detection objective without leaking test labels into threshold tuning.

## Notebook Reference
Cells 24, 29, 47, 54