# Day 05 — Exploratory Data Analysis

## Objective
Understand the distributions and fraud-related patterns in the Financial dataset before model training.

## Notebook Work
Cells 6–10 inspect sample records, unique values, numerical statistics, categorical fraud rates, feature distributions, redundancy, and numerical correlation with the fraud label.

Key findings include a Financial fraud rate of 4%, four transaction types, seven cities, five age groups, and three KYC levels. Fraud records have a higher mean transaction amount (2293.24 vs 1518.03 for normal records) and higher mean login attempts (2.16 vs 0.70).

The strongest numerical correlation with fraud is `login_attempts` (0.3126), followed by `amount` and `receiver_balance_change` (0.1025 each) and `sender_balance_change` (0.0935). The analysis also checks balance-change relationships rather than assuming that correlated fields are independent.

## Outcome
EDA identified behavioral and transaction-level signals to carry into preprocessing and modeling.

## Notebook Reference
Cells 6–10