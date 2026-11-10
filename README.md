# Feature Engineering for Cardiovascular Disease Prediction

Cardiovascular disease prediction using data preprocessing, feature engineering, and machine learning, with SHAP and LIME used to explain the predictions.

## Overview
Cardiovascular diseases are a leading cause of death worldwide, and prediction quality depends heavily on data quality. This project follows a data-centric approach: it cleans and prepares clinical data, studies feature relationships with statistical tests, trains several ML models, and explains the best model with SHAP and LIME.

## Dataset
- **Cardiovascular Disease Dataset** from a multispecialty hospital in India, accessed via [Kaggle](https://www.kaggle.com/datasets/jocelyndumlao/cardiovascular-disease-dataset)
- 1,000 subjects, 14 attributes (including the target)
- Features include age, gender, resting blood pressure, serum cholesterol, chest pain type, fasting blood sugar, maximum heart rate, exercise-induced angina, oldpeak, ST-segment slope, and number of major vessels
- Target: binary (0 = no heart disease, 1 = heart disease)
- The dataset is not included in this repository. Please download it from the link above.

## Methods
- **Preprocessing and feature engineering** on 14 clinical attributes
- **Statistical analysis:** Pearson correlation, ANOVA, Mann-Whitney U, Z-test, T-test, Chi-square
- **Models:** Random Forest, SVM, XGBoost, Logistic Regression
- **Explainable AI:** SHAP (global importance) and LIME (local explanations)

## Results

| Model | Accuracy |
|---|---|
| **Random Forest** | **98.5%** |
| SVM | 97.5% |
| XGBoost | 97.0% |
| Logistic Regression | 97.0% |

- ST-segment slope had the strongest correlation with the target (0.8), followed by chest pain type (0.55) and number of major vessels (0.49)
- SHAP identified slope, resting blood pressure, and chest pain type as the most influential features

