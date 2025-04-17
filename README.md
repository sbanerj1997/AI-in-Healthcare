# Classification Modeling with Imbalanced Dataset

Diabetes is among the most prevalent chronic diseases in the United States, impacting millions of Americans each year and exerting a significant financial burden on the economy. Diabetes is a serious chronic disease in which individuals lose the ability to effectively regulate levels of glucose in the blood, and can lead to reduced quality of life and life expectancy. This project focuses on building and evaluating classification models for an imbalanced dataset using a combination of resampling techniques, dimensionality reduction, and machine learning models including neural networks, Random Forest, and XGBoost.

# About DataSet

The target variable has 3 classes. 0 is for no diabetes, 1 is for prediabetes, and 2 is for diabetes
[Diabetes Health Indicators Kaggle Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv)

## Steps Followed

### Data Preprocessing
1. **Train-Test Split**
2. **PCA (Principal Component Analysis)**
3. **SMOTE (Synthetic Minority Over-sampling Technique)**
4. **ADASYN (Adaptive Synthetic Sampling)**

## Model Tuning
- **Bayesian Optimization** was used for hyperparameter tuning to improve model performance.

## Machine Learning Models Used
- **Random Forest (RF)**
- **XGBoost**

## Neural Network Experiments

### 1. **Without Resampling**
- Neural network applied directly on the imbalanced dataset.
- *Result:* Class 1 was poorly predicted due to imbalance.

### 2. **SMOTE (Without Scaling or PCA)**
- SMOTE applied to the training data without applying scalar or PCA.
- Neural network trained and tested on this data.

### 3. **ADASYN (Without Scaling or PCA)**
- ADASYN resampling applied to the training data.
- Neural network evaluated using this resampled data.

## Observations
- Resampling techniques like **SMOTE** and **ADASYN** improved model performance for underrepresented classes.
- Bayesian optimization significantly boosted the performance of ensemble models (RF, XGBoost).

## To Do
- Further tune neural network architecture and batch sizes.
- Work on getting better accuracy by exploring/implementing more models.

## Requirements
- Python 3.x
- scikit-learn
- imbalanced-learn
- xgboost
- pandas, numpy
- matplotlib, seaborn
- tensorflow
- optuna

## YOUTUBE LINK
[Diabetes Prediction](https://youtu.be/avh_v0ezsQ4)