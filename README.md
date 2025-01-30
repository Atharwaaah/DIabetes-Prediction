# ❤️ Heart Disease Prediction Project  
**Predicting cardiovascular events using clinical data with 86.4% accuracy**  
*ML workflow comparing 6 algorithms with integrated dataset analysis*

---

## 📋 Project Overview
This Jupyter notebook demonstrates a complete machine learning workflow using the `heart.csv` clinical dataset containing 918 patient records with 11 diagnostic features. The project achieves **86.4% accuracy** using Random Forest classification.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/atharwaaah/heart-disease-prediction/blob/main/HeartDiseasePrediction.ipynb)


---

## 🚀 Key Features
- **6 ML Algorithms Tested**  
  <img src="https://img.shields.io/badge/Random_Forest-86.4%25-brightgreen" alt="RF Accuracy"> <img src="https://img.shields.io/badge/XGBoost-85.2%25-yellowgreen" alt="XGB Accuracy">
  - Random Forest Classifier
  - XGBoost Classifier
  - Logistic Regression
  - K-Nearest Neighbors
  - Support Vector Machine
  - Decision Tree

- **Dataset Features**  
Age,Sex,ChestPainType,RestingBP,Cholesterol,FastingBS,RestingECG,MaxHR,ExerciseAngina,Oldpeak,ST_Slope,HeartDisease
| Clinical Parameter       | Description                          | Data Type |
|-------------------------|--------------------------------------|-----------|
| Age                     | Patient's age in years              | Integer   |
| RestingBP               | Resting blood pressure (mm Hg)       | Integer   |
| Cholesterol             | Serum cholesterol (mg/dl)           | Integer   |
| MaxHR                   | Maximum heart rate achieved          | Integer   |
| ExerciseAngina          | Exercise-induced angina (Y/N)        | Binary    |

---

## 🛠️ Installation
1. Clone repository:
git clone https://github.com/yourusername/heart-disease-prediction.git
cd heart-disease-prediction
2. Install requirements:
   pip install -r requirements.txt
3. Launch Jupyter notebook with dataset:
   jupyter notebook HeartDiseasePrediction.ipynb heart.csv

   
---

## 🔍 Data Exploration
The included `heart.csv` contains:
- 918 patient records
- 11 clinical features
- Binary classification (HeartDisease 0/1)

import pandas as pd
df = pd.read_csv('heart.csv')
print(f"Dataset shape: {df.shape}")
print(f"Positive cases: {df.HeartDisease.value_counts()1} ({(df.HeartDisease.value_counts()1/len(df))*100:.1f}%)")


---

## 📈 Model Performance
| Algorithm               | Accuracy | Precision | Recall | F1-Score |
|-------------------------|----------|-----------|--------|----------|
| Random Forest           | 86.4%    | 0.87      | 0.85   | 0.86     |
| XGBoost                 | 85.2%    | 0.84      | 0.83   | 0.84     |
| Logistic Regression     | 82.7%    | 0.81      | 0.80   | 0.81     |

*Detailed confusion matrices and ROC curves available in notebook*

---

## 🧠 Sample Prediction

from sklearn.preprocessing import StandardScaler
import joblib
model = joblib.load('heart_disease_model.pkl')
scaler = joblib.load('scaler.pkl')
Input features: [Age, Sex, ChestPainType, RestingBP...]
sample_data = [[40, 'M', 'ATA', 140, 289, 0, 'Normal', 172, 'N', 0, 'Up']]
processed_data = preprocess(sample_data) # Custom preprocessing function
scaled_data = scaler.transform(processed_data)
prediction = model.predict(scaled_data)
print('❤️ Healthy Heart' if prediction == 0 else '⚠️ Heart Disease Detected')


---

## 🤝 Contribution Guidelines
1. Fork the repository
2. Create your feature branch:
git checkout -b feature/AmazingFeature
3. Commit changes:
git commit -m 'Add some AmazingFeature'
4. Push to branch:
git push origin feature/AmazingFeature
5. Open a Pull Request

*Always keep original `heart.csv` intact when modifying data*

---

## 📜 License
Distributed under the MIT License. See `LICENSE` for details.

---

**Made with ❤️ by Atharv Gupta**  



