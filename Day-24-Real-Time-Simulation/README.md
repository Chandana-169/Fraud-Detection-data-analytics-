# Day 24 — Real-Time Simulation

## Objective
Simulate incoming transactions and test whether the deployed prediction function can generate fraud alerts as transactions arrive.

## Notebook Work
Cells 94–97 implement a transaction simulator, run a normal Financial stream, then run a mixed stream containing normal and known fraud transactions. The mixed experiment processes 20 transactions: 10 normal and 10 fraud.

The mixed run produced **4 true positives, 0 false positives, 10 true negatives, and 6 false negatives**, giving precision 1.00, recall 0.40, and F1 about 0.571.

## Important Note
The random-normal simulation is a pipeline smoke test, not a meaningful performance benchmark because it contains no fraud examples.

## Outcome
A working in-notebook real-time simulation was demonstrated using the saved fraud-prediction logic.

## Notebook Reference
Cells 94–97