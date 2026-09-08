# Day 27 — Streamlit Setup

## Objective
Prepare the interactive web dashboard environment from the trained fraud-detection package.

## Notebook Work
Cell 122 creates an `app.py` Streamlit application that loads saved preprocessors, models, anomaly scalers, and final model configuration. Cell 123 installs Streamlit and Pyngrok. Cells 124A/124B check the local Streamlit server and configure ngrok.

The first server check reports that Streamlit was not running at that moment; ngrok authentication configuration is included in the notebook.

## Outcome
The dashboard application file and supporting web-deployment tooling were prepared in Colab.

## Notebook Reference
Cells 122–124B