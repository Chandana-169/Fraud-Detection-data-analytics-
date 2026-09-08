# Day 06 — Behavioural Analysis

## Objective
Identify transaction behaviors that distinguish normal activity from potentially fraudulent activity.

## Notebook Work
The Financial analysis compares normal and fraud groups across transaction amount, account age, balance changes, time variables, and login behavior. Categorical fraud rates are also compared for transaction type, age group, city, and KYC level.

The clearest behavioral signal is repeated login activity. Fraud rate rises from **1.03% at 0 login attempts** to **44.36% at 4**, **82.86% at 5**, **86.67% at 6**, and **100% at 7–8** in the analyzed Financial data. Fraud transactions also show higher average amounts and larger balance changes.

## Outcome
The analysis established login attempts, transaction amount, balance changes, and account age as useful behavioral signals for subsequent fraud models.

## Notebook Reference
Cells 7–12