# 🍷 Wine Classification – Supervised Learning Project

This project was developed as part of a university Machine Learning assignment.  
The goal is to classify wine types (class 0, 1, or 2) based on 13 chemical properties from the UCI Wine dataset using various supervised learning techniques.

---

## 📊 Dataset Overview

- **Samples:** 178 wine entries  
- **Features:** 13 numerical chemical attributes (e.g., alcohol, flavanoids, color intensity)  
- **Target:** Wine class label – one of three types (0, 1, 2)  

---

## 🛠 Project Steps & Methodology

1. **Data Exploration & Preprocessing**  
   - Inspected data structure and class distribution  
   - Visualized correlations (heatmap), feature distributions (boxplots, histplots, scatterplots)  
   - Identified helpful features for classification (e.g., alcohol, color intensity)

2. **Modeling Approaches**  
   - Built and compared three pipelines using `GridSearchCV` with 5-fold cross-validation:
     - Logistic Regression + StandardScaler  
     - Random Forest + StandardScaler  
     - Random Forest + SelectKBest (feature selection)  
   - Evaluation metric: **Macro F1-score** (to address class imbalance)

3. **Model Selection**  
   - Compared F1 scores to select the best-performing model and parameter set

4. **Final Training & Test Evaluation**  
   - Retrained the selected model on full training data  
   - Evaluated predictions on unseen test data  
   - Checked for data leakage to confirm test validity

---

## 🥇 Results

- **Best model:** Random Forest with all features (StandardScaler, no feature selection)  
- **Test F1 Score:** 0.9732 – indicating balanced and strong performance across all classes  
- No duplicate rows between train and test sets were found

---

## 🧰 Tools & Libraries

- Python, scikit-learn, pandas, seaborn, matplotlib  
- Jupyter Notebook

---

## 📁 Files Included

- `Assignment2_supervised_learning_flow.ipynb` – Full project notebook  
- `wine_train.csv` & `wine_test.csv` – Training and testing datasets  
- `wine_classification_project_video.mp4` – Video explanation  
- `README.md` – This summary

---

