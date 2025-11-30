# Titanic Survival Prediction  
*A complete end-to-end Machine Learning analysis based on the Kaggle "Titanic – Machine Learning from Disaster" competition.*

## Overview
This project explores the famous Titanic dataset from Kaggle and builds a Machine Learning model to predict passenger survival.  
The notebook includes:

- Exploratory Data Analysis (EDA)  
- Feature engineering (Deck extraction, FamilySize, IsAlone, Cabin reconstruction)  
- Handling missing values (Age, Fare, Embarked, Cabin)  
- Data visualization with Plotly  
- Model training and evaluation  
- Hyperparameter tuning with GridSearchCV  
- Final prediction on the official Kaggle test set  
- Submission file creation and result analysis  

This is my first full Kaggle notebook and represents a hands-on learning journey through data storytelling, feature engineering and modelling.

---

## Project Goals
- Understand the structure and challenges of the Titanic dataset  
- Identify meaningful patterns behind survival rates  
- Build a consistent and well-documented ML pipeline  
- Learn how to submit predictions to Kaggle  
- Compare predicted survival trends with real training-set distributions  
- Achieve a competitive submission score

---

## Feature Engineering Highlights
This project includes several custom techniques to enrich the dataset:

### Cabin & Deck Reconstruction  
- Extracted deck letters from Cabin strings  
- Imputed missing deck values using ticket grouping and fare consistency  
- Added `Deck_imputed_*` dummy variables  

### Family-Based Features  
- Created `FamilySize = SibSp + Parch + 1`  
- Created `IsAlone` as a high-signal indicator  

### Fare & Embarkment Cleaning  
- Log-transformation of Fare (`Fare_log`)  
- Imputation of missing Embarked values via fare distribution analysis  

### Comparison Plots  
After predictions, the notebook recombines the `test.csv` data with the predicted survival values and compares Age–Survival trends between training data and predicted data to evaluate consistency.

---

## Modelling
The final model is a **Random Forest Classifier**, optimized via GridSearchCV.

**Best hyperparameters:**
- `max_depth = 10`
- `min_samples_split = 2`
- `n_estimators = 100`

The model was retrained on **100% of the training data** before generating predictions for Kaggle.

---

## Kaggle Submission
A submission CSV was generated and uploaded to the competition.

**Final Kaggle public score:** **0.75598**

This is aligned with many baseline-plus feature-engineering approaches for Titanic and demonstrates a solid first complete ML pipeline.

---

# 🚢 Titanic Survival Prediction  
*A complete end-to-end Machine Learning analysis based on the Kaggle "Titanic – Machine Learning from Disaster" competition.*

## 📌 Overview
This project explores the famous Titanic dataset from Kaggle and builds a Machine Learning model to predict passenger survival.  
The notebook includes:

- Exploratory Data Analysis (EDA)  
- Feature engineering (Deck extraction, FamilySize, IsAlone, Cabin reconstruction)  
- Handling missing values (Age, Fare, Embarked, Cabin)  
- Data visualization with Plotly  
- Model training and evaluation  
- Hyperparameter tuning with GridSearchCV  
- Final prediction on the official Kaggle test set  
- Submission file creation and result analysis  

This is my first full Kaggle notebook and represents a hands-on learning journey through data storytelling, feature engineering and modelling.

---

## 🎯 Project Goals
- Understand the structure and challenges of the Titanic dataset  
- Identify meaningful patterns behind survival rates  
- Build a consistent and well-documented ML pipeline  
- Learn how to submit predictions to Kaggle  
- Compare predicted survival trends with real training-set distributions  
- Achieve a competitive submission score

---

## 🧪 Feature Engineering Highlights
This project includes several custom techniques to enrich the dataset:

### ✔️ Cabin & Deck Reconstruction  
- Extracted deck letters from Cabin strings  
- Imputed missing deck values using ticket grouping and fare consistency  
- Added `Deck_imputed_*` dummy variables  

### ✔️ Family-Based Features  
- Created `FamilySize = SibSp + Parch + 1`  
- Created `IsAlone` as a high-signal indicator  

### ✔️ Fare & Embarkment Cleaning  
- Log-transformation of Fare (`Fare_log`)  
- Imputation of missing Embarked values via fare distribution analysis  

### ✔️ Comparison Plots  
After predictions, the notebook recombines the `test.csv` data with the predicted survival values and compares Age–Survival trends between training data and predicted data to evaluate consistency.

---

## 📊 Modelling
The final model is a **Random Forest Classifier**, optimized via GridSearchCV.

**Best hyperparameters:**
- `max_depth = 10`
- `min_samples_split = 2`
- `n_estimators = 100`

The model was retrained on **100% of the training data** before generating predictions for Kaggle.

---

## 🏁 Kaggle Submission
A submission CSV was generated and uploaded to the competition.

**Final Kaggle public score:** **0.75598**

This is aligned with many baseline-plus feature-engineering approaches for Titanic and demonstrates a solid first complete ML pipeline.

---


## 🧑‍💻 Author
**Luca Scarpantonio**  
Data Science & Machine Learning Enthusiast  
GitHub: *[Luca on GitHub](https://lucascarpantonio.github.io/)*
Kaggle: *[Luca on Kaggle](https://www.kaggle.com/lucascarpantonio)*  

