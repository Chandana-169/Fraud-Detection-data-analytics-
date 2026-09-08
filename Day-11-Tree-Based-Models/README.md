# Day 11 — Tree-Based Models

## Objective
Compare tree-based classifiers with the Logistic Regression baseline.

## Notebook Work
Cell 26 trains a Decision Tree and Cell 27 trains a Random Forest on the processed training data. Validation precision, recall, F1, and PR-AUC are used to compare their fraud-detection behavior.

Validation F1 results included approximately **0.594 Credit / 0.209 Financial / 0.557 Synthetic / 0.831 Orders** for the Decision Tree, while Random Forest achieved approximately **0.779 Credit / 0.271 Financial / 0.762 Synthetic / 0.896 Orders**.

## Outcome
Random Forest improved over the Decision Tree on the validation sets, but the Financial dataset remained difficult. The tree-based comparison also provided a benchmark for the later XGBoost and hybrid approach.

## Notebook Reference
Cells 26–27