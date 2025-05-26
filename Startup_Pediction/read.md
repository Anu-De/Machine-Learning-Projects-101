# Model Performance Analysis

## Overview
This project involves data exploration, preprocessing, model training, hyperparameter tuning, and evaluation for a classification task. The goal was to identify the best-performing model based on various metrics such as accuracy, ROC AUC, and PR AUC.

## Data Exploration
We visualized feature relationships using correlation heatmaps, distribution plots, box-whisker plots, and scatter matrices to understand data characteristics and identify outliers.

## Models and Tuning
We trained and optimized three models:
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- XGBoost

Hyperparameters were tuned using grid search to find the optimal configurations for each model.

## Results and Conclusions

Our evaluation indicates that **XGBoost** outperforms the other models across all key metrics, demonstrating strong predictive power and robustness.

### Model Performance Summary

| Model        | Best Hyperparameters                                                                 | Training Accuracy | Testing Accuracy | ROC AUC | PR AUC | Remarks                                    |
|--------------|--------------------------------------------------------------------------------------|---------------------|------------------|---------|--------|--------------------------------------------|
| **KNN**    | metric: Manhattan, n_neighbors: 9, weights: uniform                                | 80.51%             | 82.74%          | 0.852  | 0.919 | Moderate performance, sensitive to outliers |
| **SVC**    | C: 1, gamma: auto                                                                   | 82.88%             | 83.93%          | 0.860  | 0.923 | Slightly better than KNN, still room for improvement |
| **XGBoost**| colsample_bytree=1, gamma=0.1, learning_rate=0.1, max_depth=3, n_estimators=100, subsample=1 | 93.75%             | 90.48%          | 0.926  | 0.958 | Best overall performance, robust and reliable |

## Summary
The XGBoost model demonstrated the highest accuracy and AUC scores, making it the most effective for this classification problem. Its high generalization ability suggests it is the ideal candidate for deployment or further tuning.
