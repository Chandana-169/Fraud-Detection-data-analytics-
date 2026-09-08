# Day 20 — Transaction Investigation

## Objective
Turn model predictions into an investigation-oriented view of suspicious transactions.

## Notebook Work
The notebook includes a dedicated Day 20 investigation block after the initial dashboard/deployment cells. It uses the selected models and thresholds for Credit, Financial, Synthetic, and Orders, generates fraud probabilities, assigns High/Medium/Low risk, and compares predictions with actual labels.

Each investigated transaction receives a status: **Confirmed Fraud**, **Potential False Positive**, **Missed Fraud**, or **Normal**. Results are sorted by fraud probability and the top suspicious transactions are displayed. An overall investigation summary is also saved as `transaction_investigation_summary.csv`.

## Outcome
The project moves from model scores to an analyst-facing investigation table that separates confirmed detections, false positives, missed fraud, and normal transactions.

## Notebook Reference
Dedicated Day 20 block following Cell 124B