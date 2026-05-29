# MLOps Capstone Architecture

## Overview

This project implements an end-to-end MLOps pipeline using Databricks and MLflow.

## Architecture Flow

1. **Data Ingestion**
   - Dataset loaded using scikit-learn
   - Converted to Spark DataFrame
   - Stored as a managed Delta table in Databricks

2. **Exploratory Data Analysis**
   - Performed using PySpark and Pandas API on Spark
   - Feature distributions and data quality reviewed

3. **Model Training & Experiment Tracking**
   - Multiple Random Forest models trained
   - MLflow used for experiment tracking
   - Metrics logged: Accuracy, F1 score, ROC AUC

4. **Model Registry**
   - Best model selected based on ROC AUC
   - Model registered in MLflow Model Registry
   - Lifecycle managed using aliases (`@challenger`, `@champion`)

5. **Model Serving**
   - Champion model deployed to Databricks Model Serving
   - Real-time REST endpoint created
   - Endpoint tested using an external Python client

## Key Technologies

- Databricks
- Apache Spark
- MLflow
- scikit-learn
- Python