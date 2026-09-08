# Day 02 — Dataset Audit

## Objective
Audit the four fraud-detection datasets before modeling and understand their structure, target labels, class balance, columns, and data types.

## Notebook Work
Cells 2–5 upload and inspect the datasets. The notebook loads Credit, Financial, Synthetic, and Orders data and performs a common quality check for rows, columns, missing values, duplicates, target name, normal records, fraud records, and fraud percentage.

Cell 5 then lists every column and its data type for each dataset. The audit reveals that the datasets have different schemas and target-column names (`IsFraud` for Credit and `is_fraud` for the other datasets).

## Key Results
- Credit: 18,000 rows, 19 columns, 720 fraud records (4%).
- Financial: 16,000 rows, 19 columns, 640 fraud records (4%).
- Synthetic: 18,000 rows, 18 columns, 720 fraud records (4%).
- Orders: 15,000 rows, 19 columns, 600 fraud records (4%).
- Missing values: 0 in all four datasets.
- Duplicate rows: 0 in all four datasets.

## Outcome
The audit confirmed that all four files were usable for the modeling workflow while still requiring dataset-specific preprocessing because their feature sets and data types differ.

## Notebook Reference
Cells 2–5