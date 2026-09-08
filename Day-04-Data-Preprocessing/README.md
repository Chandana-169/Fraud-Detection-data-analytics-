# Day 04 — Data Preprocessing

## Objective
Prepare the four datasets for machine-learning models while preserving useful categorical and numerical information.

## Notebook Work
Cells 14–22 create clean modeling datasets, separate features and targets, identify numerical/categorical columns, build preprocessing pipelines, and handle the Credit dataset's `MerchantID` correctly.

The preprocessing workflow uses `ColumnTransformer`/`Pipeline` and encodes categorical features while scaling numerical features. `MerchantID` is explicitly changed from numerical to categorical because it is an identifier rather than a continuous measurement. Credit preprocessing is then rebuilt and SMOTE is reapplied.

## Outcome
Dataset-specific processed feature matrices were produced. The final processed dimensions include approximately 429 Credit features, 32 Financial features, 30 Synthetic features, and 36 Orders features after encoding.

## Notebook Reference
Cells 14–22