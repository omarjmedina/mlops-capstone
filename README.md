# MLOps Capstone Project

This repository contains an end-to-end MLOps pipeline built as a capstone project.

## Project Overview

The project demonstrates a complete machine learning lifecycle using Databricks and MLflow:

- Data ingestion and exploratory data analysis
- Experiment tracking with MLflow
- Model training and evaluation
- Model registration using Unity Catalog
- Model serving via Databricks Model Serving
- Optional sovereign AI inference using a local Rust-based APR CLI

## Repository Structure

```text
mlops-capstone/
├── dev/
│   ├── notebooks/
│   │   ├── 01_data_ingestion_eda
│   │   └── 02_train_track_register
│   └── data/
│       └── README.md
├── docs/
│   └── architecture.md
├── prod/
│   └── README.md
└── README.md
