# Project Notes (AI/ML Project Manager Perspective)

## Goals
- Validate data readiness via quality gates
- Quantify model risk using business-oriented metrics (precision/recall, cost tradeoffs)
- Detect drift and decide when to alert vs retrain
- Provide an operational monitoring layer via SQL + Tableau

## Data Quality Gates (Go/No-Go)
- Missing values: thresholds per feature group
- Schema checks: type validation, range checks
- Class imbalance: baseline rate, impact on metrics and sampling strategy
- Outliers: detection strategy and decision (cap/remove/keep)

## Model Evaluation (Business Lens)
- Accuracy is insufficient for imbalanced risk problems
- Track: precision, recall, PR-AUC, confusion matrix at chosen threshold
- Interpret: false positives (ops cost) vs false negatives (risk exposure)

## Drift Monitoring Strategy
- Feature drift: distribution shift between training vs recent scoring window
- Prediction drift: probability distribution shifts over time
- Triggers (example):
  - Alert when drift metric exceeds threshold for key features
  - Retrain when drift persists AND performance drops on a labeled sample

## Deliverables
- Notebooks documenting decisions and rationale
- SQL schema + queries for monitoring KPIs
- Tableau dashboard for stakeholders
