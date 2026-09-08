# Day 16 — Autoencoder

## Objective
Test deep-learning-based reconstruction error as an unsupervised fraud/anomaly signal.

## Notebook Work
Cells 38–42 set up TensorFlow/Keras, train an autoencoder using normal training examples, calculate reconstruction errors, optimize a validation threshold, and evaluate the resulting anomaly detector on test data.

The reconstruction-error gap between normal and fraud transactions was small for Credit and Financial and more visible for Synthetic and Orders. Final test F1 remained low: approximately **0.119 Credit, 0.074 Financial, 0.237 Synthetic, and 0.172 Orders**.

## Outcome
The autoencoder was retained as an experimental anomaly-detection approach but was not selected as a final production model.

## Notebook Reference
Cells 38–42