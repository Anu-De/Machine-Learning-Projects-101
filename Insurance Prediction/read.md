# Insurance Charges Prediction

## Project Overview
This project focuses on predicting insurance charges based on various demographic and health-related features. Using a structured data analysis and machine learning approach, the goal is to develop an accurate model that can estimate insurance costs for individuals.

## Dataset Description
The dataset used in this project contains information about individuals, including features such as age, sex, BMI, smoking status, region, and other health indicators, along with the corresponding insurance charges. This data is commonly used to understand factors influencing insurance costs and to build predictive models.

## What I Am Doing
The project involves the following steps:

1. **Data Loading and Exploration**
   - Loaded the dataset and examined its structure.
   - Performed exploratory data analysis (EDA) including:
     - Checking data info, description, missing values, duplicates, and correlations.
     - Visualizing feature distributions with histograms.
     - Detecting outliers via box plots.

2. **Data Preprocessing**
   - Encoded categorical variables using binary encoding and one-hot encoding.
   - Scaled numerical features using standard scaling techniques.
   - Split the data into training and hold-out test sets.

3. **Model Building and Hyperparameter Tuning**
   - Trained multiple regression models:
     - Linear Regression, Ridge, Lasso, ElasticNet
     - Decision Tree, Random Forest, Gradient Boosting, XGBoost
     - K-Nearest Neighbors, Support Vector Regression
   - Performed hyperparameter tuning to optimize model performance.

4. **Model Evaluation**
   - Evaluated models using metrics such as MSE, MAE, RMSE, and R².
   - Identified the best-performing models based on validation scores.

5. **Ensemble Modeling**
   - Built a stacking ensemble combining the top models to improve prediction accuracy.
   - Evaluated the stacking model on the test set, achieving high performance metrics:
     - MSE: 0.1582
     - MAE: 0.21
     - RMSE: 0.3978
     - R²: 0.82

## Conclusion
The stacking ensemble model demonstrated excellent predictive capability, capturing over 82% of the variance in insurance charges with minimal error. This approach can be utilized for insurance cost estimation and financial planning.

## Technologies & Libraries
- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- xgboost

## Future Work
- Incorporate additional features for improved accuracy.
- Explore advanced ensemble techniques.
- Deploy the model for real-time prediction applications.

---

**Note:** Ensure you have the necessary libraries installed to run this project smoothly.
