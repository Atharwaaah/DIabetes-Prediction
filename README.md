# ❤️ Heart Disease Prediction Project  
**Predicting cardiovascular events using clinical data with 86.4% accuracy**  
*ML workflow comparing 6 algorithms with integrated dataset analysis*

---

## 📋 Project Overview
This Jupyter notebook analyzes the `heart.csv` dataset containing **918 patient records** with 11 clinical features. Implements complete ML pipeline achieving **86.4% accuracy** using Random Forest.

---

## 🗃️ Dataset Structure (heart.csv)
| Column               | Description                          | Example Value |
|----------------------|--------------------------------------|---------------|
| Age                  | Patient's age in years               | 40            |
| ChestPainType        | Chest pain category (ATA/NAP/ASY/TA)  | ASY           |
| RestingBP            | Resting blood pressure (mm Hg)       | 140           |
| Cholesterol          | Serum cholesterol (mg/dl)            | 289           |
| FastingBS            | Fasting blood sugar >120 mg/dl       | 0             |
| ExerciseAngina       | Exercise-induced angina (Y/N)         | N             |

*Sample data from heart.csv:*
Age,Sex,ChestPainType,RestingBP,Cholesterol,FastingBS,RestingECG,MaxHR,ExerciseAngina,Oldpeak,ST_Slope,HeartDisease
40,M,ATA,140,289,0,Normal,172,N,0,Up,0
49,F,NAP,160,180,0,Normal,156,N,1,Flat,1
---

## 🛠️ Installation
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
pip install -r requirements.txt
**Requirements.txt**
pandas==1.5.3
scikit-learn==1.2.2
xgboost==1.7.6
matplotlib==3.7.1
---

## 🔍 Quick Start
1. Load dataset:
   import pandas as pd
   df = pd.read_csv('heart.csv')
   print(f"Dataset shape: {df.shape}")

2. Train model:
   from sklearn.ensemble import RandomForestClassifier
   model = RandomForestClassifier()
   model.fit(X_train, y_train)
   ---

## 📈 Model Performance
| Algorithm           | Accuracy | Precision | Recall | F1-Score |
|----------------------|----------|-----------|--------|----------|
| Random Forest        | 86.4%    | 0.87      | 0.85   | 0.86     |
| XGBoost              | 85.2%    | 0.84      | 0.83   | 0.84     |
| Logistic Regression  | 82.7%    | 0.81      | 0.80   | 0.81     |

---

## 📂 File Structure
├── heart.csv # Primary dataset
├── HeartFailurePrediction.ipynb # Main notebook
├── requirements.txt # Dependency list
└── README.md # This documentation
---

## 🤝 Contribution
Always preserve original dataset
cp heart.csv heart_modified.csv
*Dataset license: CC BY-NC-SA 4.0*

---

**Developed using clinical data from heart.csv**  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yourusername/heart-disease-prediction/blob/main/HeartFailurePrediction.ipynb)
