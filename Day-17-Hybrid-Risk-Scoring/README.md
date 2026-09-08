# Day 17 — Hybrid Risk Scoring

## Objective
Combine supervised fraud probability with an unsupervised anomaly signal to create a broader transaction-risk score.

## Notebook Work
Cells 43–55 compare supervised models, construct hybrid scores, classify risk, evaluate the hybrid approach, and then correct the anomaly normalization to a production-safe training-derived scale.

The hybrid score combines **70% supervised XGBoost probability + 30% normalized Isolation Forest anomaly score**. The production-safe version stores anomaly-score minimum/maximum values from training rather than deriving scaling from the test set.

Production-safe hybrid test F1 was approximately **0.824 Credit, 0.386 Financial, 0.772 Synthetic, and 0.889 Orders** before final model selection.

## Outcome
The hybrid approach improved the Credit and Financial selection relative to their supervised alternatives and became the selected model for those two datasets.

## Notebook Reference
Cells 43–55