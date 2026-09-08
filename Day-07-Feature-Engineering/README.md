# Day 07 — Feature Engineering

## Objective
Prepare meaningful numerical and categorical predictors from the four transaction datasets.

## Notebook Work
The notebook reviews feature types and builds dataset-specific modeling representations. Existing engineered Financial variables such as `transaction_month`, `transaction_day`, `transaction_dayofweek`, `transaction_hour`, `sender_balance_change`, and `receiver_balance_change` are retained as model features.

Categorical variables such as transaction type, city, age group, KYC level, merchant/category, payment method, device, and location are handled as categorical inputs. Identifier-like fields are treated carefully; in particular, Credit `MerchantID` is moved from numerical to categorical before rebuilding its preprocessing pipeline.

## Outcome
The feature-engineering stage produces consistent numerical/categorical feature definitions for each dataset and prepares them for model training without treating identifiers as continuous measurements.

## Notebook Reference
Cells 13–22