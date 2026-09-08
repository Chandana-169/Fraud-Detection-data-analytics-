# Day 03 — Dataset Selection

## Objective
Select and retain a multi-dataset fraud-detection setup that supports comparison across different transaction domains.

## Selected Datasets
The notebook uses four datasets:
1. **Credit** — 18,000 records, 19 columns.
2. **Financial** — 16,000 records, 19 columns.
3. **Synthetic** — 18,000 records, 18 columns.
4. **Orders** — 15,000 records, 19 columns.

Total records: **67,000**.

## Selection Work
Cells 3–6 load the four datasets, inspect their schemas, and perform a detailed inspection of the Financial dataset. The datasets contain different transaction attributes, allowing the project to compare fraud-detection behavior across domains rather than relying on one feature schema.

## Important Observation
All four selected datasets contain approximately 4% fraud. The notebook keeps the original records and evaluates models using fraud-sensitive metrics rather than changing the data merely to improve scores.

## Outcome
A four-dataset modeling framework was established for the remaining project stages.

## Notebook Reference
Cells 3–6