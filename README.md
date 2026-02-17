# ML Model Monitoring & Drift Analysis (Python + SQL + Tableau)

## Executive Summary
This repository demonstrates a production-like ML monitoring workflow from an AI/ML Project Manager perspective:
- Data quality gates (Go/No-Go checks)
- Model training & business-oriented evaluation
- Batch inference simulation
- Feature & prediction drift detection
- SQL-based monitoring layer
- Tableau dashboard for decision support

## Problem Framing (Why Monitoring)
ML models degrade when data distributions shift. Drift can increase false positives/negatives, creating operational cost and business risk.
This project shows how to detect drift and translate it into actionable decisions (alerts, investigation, retraining).

## Tech Stack
- Python: pandas, numpy, scikit-learn
- SQL: MySQL (or compatible)
- Tableau: monitoring dashboard

## Repository Structure
- `notebooks/` : analysis notebooks (end-to-end)
- `sql/` : schema + monitoring queries
- `src/` : reusable pipeline code
- `tableau/` : dashboard exports (PNG)
- `data/` : folder structure only (raw/processed ignored)

## Notebooks
1. `01_data_quality_analysis.ipynb` — data quality gates, imbalance checks, outliers
2. `02_model_training_evaluation.ipynb` — baseline model + threshold tradeoffs
3. `03_prediction_simulation.ipynb` — batch scoring + persistence
4. `04_drift_detection_analysis.ipynb` — drift metrics + operational interpretation

## Dashboard
Add `tableau/monitoring_dashboard.png` and reference it here once created.
