# Day 26 — Fraud Alerts

## Objective
Convert model probabilities into actionable fraud-risk alerts.

## Notebook Work
Cells 60–64 generate fraud alerts from the selected final models. Each transaction receives a fraud probability, prediction, risk level, and alert indicator. The workflow distinguishes **High, Medium, and Low** risk.

The alert system is applied across Credit, Financial, Synthetic, and Orders datasets, and alert-performance summaries are created. The final alert CSV files are also saved for downstream reporting.

## Outcome
The project moves from model evaluation to an operational alert layer that can flag suspicious transactions for review.

## Notebook Reference
Cells 60–64 and final prediction/alert generation in Cell 70