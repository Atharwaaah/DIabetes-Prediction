# Diabetes-Prediction
# Diabetes Prediction using Machine Learning

## Overview
This project implements a Logistic Regression model to predict diabetes in patients using diagnostic measurements from the National Institute of Diabetes and Digestive and Kidney Diseases dataset.

## Dataset Features
| Feature | Description | Type |
|---------|-------------|------|
| Pregnancies | Number of times pregnant | Numeric |
| Glucose | Plasma glucose concentration | Numeric |
| BloodPressure | Diastolic blood pressure (mm Hg) | Numeric |
| SkinThickness | Triceps skin fold thickness (mm) | Numeric |
| Insulin | 2-Hour serum insulin (mu U/ml) | Numeric |
| BMI | Body mass index | Numeric |
| DiabetesPedigreeFunction | Diabetes pedigree function | Numeric |
| Age | Age in years | Numeric |
| Outcome | Diabetes diagnosis (0/1) | Binary |

## Model Implementation
- **Algorithm:** Logistic Regression
- **Data Preprocessing:** Standardization using Z-score normalization
- **Feature Scaling:** StandardScaler from scikit-learn
- **Train-Test Split:** 80-20 ratio

## Key Steps
1. Data loading and exploration
2. Feature standardization/normalization
3. Model training and evaluation
4. Prediction on test data

## Requirements
numpy==1.21.5
pandas==1.4.2
scikit-learn==1.0.2

## Usage
python diabetes_prediction.py

## License
MIT License

