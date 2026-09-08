# Day 25 — Kafka Pipeline

## Notebook Status
A real Apache Kafka broker/producer/consumer pipeline is **not implemented and executed** in the verified notebook.

## What Is Present
The notebook contains an in-memory queue and threaded producer/consumer implementation in Cells 107–114. It simulates streaming transactions and passes them through the fraud-prediction function.

The original project specification mentions Kafka/Spark Streaming, but the completed notebook uses the local queue/threading prototype instead of a live Kafka cluster.

## Outcome
The project demonstrates the streaming architecture concept and validates producer/consumer behavior, but this should not be described as a production Kafka deployment.

## Notebook Reference
Cells 107–114