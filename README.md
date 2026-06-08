# Predictive Maintenance System using Machine Learning

## Business Problem

Unexpected machine failures can lead to production downtime,
increased maintenance costs, and operational disruptions.

The objective of this project is to predict machine failures
using operational sensor data and identify the most important
factors contributing to failure risk.

## Dataset

AI4I 2020 Predictive Maintenance Dataset

Features:
- Air Temperature
- Process Temperature
- Rotational Speed
- Torque
- Tool Wear
- Machine Type

Target:
- Machine Failure

## Key Findings

- Low-quality machines exhibited higher failure rates.
- Torque was strongly associated with machine failure.
- Tool wear increased failure risk.
- Machine failures represented only 3.39% of observations.

## Models

1. Logistic Regression
2. Random Forest
3. XGBoost

## Results

| Model | Precision | Recall | F1 | ROC-AUC |
|---------|---------:|---------:|---------:|---------:|
| Logistic Regression | 0.14 | 0.82 | 0.25 | 0.91 |
| Random Forest | 0.79 | 0.71 | 0.74 | 0.96 |
| XGBoost | 0.42 | 0.84 | 0.56 | 0.97 |

## Model Selection

Random Forest was selected as the final model.

Although XGBoost achieved the highest ROC-AUC score,
Random Forest achieved a superior balance between
precision and recall after threshold tuning.

Final Performance:

- Precision: 78.7%
- Recall: 70.6%
- F1 Score: 74.4%
- ROC-AUC: 96.3%

## Business Impact

A predictive maintenance system can help identify
high-risk machines before failure occurs.

Benefits include:

- Reduced unplanned downtime
- Lower maintenance costs
- Improved operational reliability
- Better maintenance scheduling
