# Data Directory

This directory is reserved for small reference datasets, schemas, or sample inputs.

In this project, the primary dataset is loaded directly into Databricks
and stored as a managed Delta table (`workspace.default.breast_cancer`)
instead of local files.

This approach aligns with Databricks best practices for scalable data access.