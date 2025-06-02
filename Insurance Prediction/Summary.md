### **Conclusion**

In this project, we explored and analyzed the dataset through various visualization techniques, including correlation heatmaps, distribution plots, box-whisker plots, and scatter matrices to understand feature relationships and identify potential outliers. Following data preprocessing steps such as missing value handling, feature scaling, and encoding, we trained three different models: K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), and XGBoost.

Hyperparameter tuning was performed using grid search, leading to the selection of optimal parameters for each model. The evaluation metrics across these models revealed that **XGBoost consistently outperformed KNN and SVC** in terms of accuracy, ROC AUC, and PR AUC. Specifically, the XGBoost model achieved a testing accuracy of **90.48%**, ROC AUC of **0.926**, and PR AUC of **0.958**, indicating excellent discrimination ability and robustness.

Given its superior performance and minimal overfitting, **XGBoost was identified as the best model** for this classification task. Its high feature importance scores further suggest that the model effectively captures relevant patterns in the data, making it suitable for deployment or further analysis.

---

### **Model Performance Comparison**

| Model        | Best Hyperparameters                                                                 | Training Accuracy | Testing Accuracy | ROC AUC | PR AUC | Remarks                                    |
|--------------|--------------------------------------------------------------------------------------|---------------------|------------------|---------|--------|--------------------------------------------|
| **KNN**    | metric: Manhattan, n_neighbors: 9, weights: uniform                                | 80.51%             | 82.74%          | 0.852  | 0.919 | Moderate performance, sensitive to outliers |
| **SVC**    | C: 1, gamma: auto                                                                   | 82.88%             | 83.93%          | 0.860  | 0.923 | Slightly better than KNN, still room for improvement |
| **XGBoost**| colsample_bytree=1, gamma=0.1, learning_rate=0.1, max_depth=3, n_estimators=100, subsample=1 | 93.75%             | 90.48%          | 0.926  | 0.958 | Best overall performance, robust and reliable |

---

**Summary:**  
The XGBoost model demonstrated the highest accuracy and AUC scores, making it the most effective for this classification problem. Its ability to generalize well suggests it is the preferred choice for deployment or further tuning.
