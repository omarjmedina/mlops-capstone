# Production Artifacts

This directory represents production-facing assets.

In this capstone project:
- Models are promoted to production using MLflow model aliases (`@champion`)
- Production inference is handled via Databricks Model Serving endpoints
- No standalone production notebooks are required

The serving endpoint `breast-cancer-classifier-endpoint` represents the
production deployment of the model.