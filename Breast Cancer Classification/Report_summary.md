Project Report: Breast Cancer Classification

1. Dataset Overview
The dataset used in this project pertains to breast cancer diagnosis, with the primary target variable being diagnosis, categorized as B (Benign) and M (Malignant). The dataset comprised mostly numerical features, with the exception of the diagnosis label.

2. Data Exploration and Preprocessing  

    Initial Exploration: Conducted data exploration using isnull(), duplicated(), info(), describe(), and head() to understand data structure and identify missing values or duplicates.
    Outlier Detection: Outliers were identified and removed using the Interquartile Range (IQR) method.
    Skewness Handling: Checked skewness for numerical features; applied log transformation to correct skewness and validated the effectiveness post-transformation.
    Feature Scaling: Transformed numerical columns using StandardScaler to normalize feature ranges.

3. Model Training and Evaluation
Four different classification algorithms were employed:

    Logistic Regression:

   
        Achieved an accuracy of approximately 97.75%
        ROC AUC score of 0.998
        Performance metrics indicate high precision, recall, and F1-score for both classes.

    K-Nearest Neighbors (KNN):

   
        Best parameters: n_neighbors=23, p=2, weights='uniform'
        Accuracy of 96.63%
        ROC AUC of 0.996

    Decision Tree:

   
        Best parameters: criterion='entropy', max_depth=3, min_samples_leaf=4
        Accuracy of 93.25%
        ROC AUC of 0.944

    Random Forest:

   
        Best parameters: n_estimators=200, max_features='log2', min_samples_leaf=2
        Accuracy of 95.51%
        ROC AUC of 0.993

    XGBoost:

   
        Best parameters: n_estimators=100, max_depth=3, learning_rate=0.2
        Accuracy of 96.63%
        ROC AUC of 0.995

5. Comparative Analysis
All models demonstrated strong performance, with Logistic Regression and XGBoost yielding the highest accuracy and ROC AUC scores. The results indicate that these models are highly effective in distinguishing between benign and malignant tumors.

6. Conclusion
The project successfully implemented a comprehensive data exploration, preprocessing, and modeling pipeline for breast cancer classification. The models achieved high accuracy and ROC AUC scores, suggesting reliable predictive performance. Logistic Regression and XGBoost emerged as the top-performing algorithms, suitable for deployment in diagnostic support systems. Future work could involve feature importance analysis, ensemble methods, and validation on external datasets to further enhance model robustness.
