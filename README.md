# Financial Fraud Detection Model with Dashboard

## Project Overview
This project develops a machine-learning-based financial fraud detection system using multiple transaction datasets. The workflow covers data auditing, preprocessing, exploratory and behavioral analysis, supervised and unsupervised learning, hybrid risk scoring, explainability, transaction investigation, network analysis, streaming simulation, fraud alerts, adaptive learning, and an interactive Streamlit dashboard.

## Datasets
The project uses four datasets:
- Credit
- Financial
- Synthetic
- Orders

## Machine Learning
### Supervised Models
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Support Vector Machine (SVM)

### Unsupervised Models
- Isolation Forest
- One-Class SVM
- Autoencoder

### Hybrid Risk Scoring
The final workflow combines supervised fraud probability with an Isolation Forest anomaly signal for selected datasets.

## Explainability and Investigation
The project includes SHAP-based explainability, transaction-level investigation, false-positive/false-negative analysis, and graph/network analysis of transaction relationships.

## Streaming and Alerts
A transaction streaming prototype processes transactions sequentially and generates fraud predictions, risk levels, and alerts. The current streaming implementation is a prototype/simulation rather than a deployed Kafka production cluster.

## Adaptive Learning
Batch-based fraud-rate monitoring and drift detection are included to assess changes in fraud patterns over time.

## Dashboard
A Streamlit dashboard provides interactive fraud prediction functionality across the project datasets using the saved model package.

## Project Structure
The project is organized into 30 development days:

1. Project Setup
2. Dataset Audit
3. Dataset Selection
4. Data Preprocessing
5. EDA
6. Behavioural Analysis
7. Feature Engineering
8. Data Splitting
9. Class Imbalance
10. Logistic Regression
11. Tree-Based Models
12. XGBoost
13. Optuna Optimization
14. SVM Model Comparison
15. Isolation Forest
16. Autoencoder
17. Hybrid Risk Scoring
18. Risk Thresholds
19. SHAP Explainability
20. Transaction Investigation
21. Model Calibration
22. Cross-Dataset Validation
23. Error Analysis
24. Real-Time Simulation
25. Kafka / Streaming Pipeline
26. Fraud Alerts
27. Streamlit Setup
28. Streamlit Dashboard
29. Real-Time Dashboard Integration
30. Final Integration

## Final Model Selection
The final workflow uses dataset-specific model selection and thresholds. Credit and Financial use the Hybrid Model, while Synthetic and Orders use Logistic Regression.

## Limitations
- The streaming implementation is an in-memory prototype rather than a deployed Kafka/Spark production pipeline.
- The graph/network structure is a demonstration based on the available project data and should not be interpreted as proof of real-world fraud rings.
- Model selection and evaluation should be interpreted within the project's current validation and test workflow.

## Future Improvements
- Deploy a production Kafka/Spark Streaming pipeline.
- Connect live streaming outputs directly to the dashboard.
- Expand graph analysis using real entity relationships.
- Add continuous model retraining and monitoring in production.
