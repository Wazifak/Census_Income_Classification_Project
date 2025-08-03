# 📊 Census Income Classification

This machine learning project aims to predict whether a person earns more than $50,000 a year based on their demographic and economic attributes. It uses the UCI Census Income dataset and evaluates different classification models for performance.

---

## 📁 Dataset Overview

- Source: [UCI Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult)
- Total Records: ~48,000 (after cleaning)
- Features:
  - `age`, `workclass`, `education`, `marital-status`, `occupation`, `relationship`, `race`, `sex`, `capital-gain`, `capital-loss`, `hours-per-week`, `native-country`
- Target: `income`
  - `0 = <=50K`
  - `1 = >50K` (high income)

---

## 🎯 Objectives

- Understand income inequality patterns using ML
- Clean and preprocess real-world census data
- Train classification models to predict high-income individuals
- Compare model performance using accuracy and F1-score

---

## ✅ Workflow Summary

### 1. Data Preprocessing
- Removed records with missing values
- Applied label encoding on categorical columns
- Standardized numerical features (`age`, `hours-per-week`, etc.)
- Target column mapped: `<=50K → 0`, `>50K → 1`

### 2. Data Splitting
- Train-test split: 70% training, 30% testing
- Stratified sampling to maintain income ratio

### 3. Model Training
- Trained 3 models:
  - Logistic Regression
  - Decision Tree
  - Random Forest

### 4. Evaluation Metrics
- Confusion matrix
- Classification report (precision, recall, F1-score)
- Accuracy

---

## 📊 Model Performance

### 🔹 Logistic Regression
- **Accuracy**: `82.48%`
- **Confusion Matrix**:
- [[4604 301]
- [839 764]]

- ---

- **Class 1 (High Income) Metrics**:
- Precision: 0.72
- Recall: 0.48
- F1-score: 0.57

### 🔹 Decision Tree
- **Accuracy**: `81.11%`
- **Confusion Matrix**:
[[4280 625]
[ 604 999]]

---
- **Class 1 (High Income) Metrics**:
- Precision: 0.62
- Recall: 0.62
- F1-score: 0.62

### 🔹 Random Forest (best model)
- **Accuracy**: ~`85%`
- **Macro F1-score**: ~0.78
- **Insight**: Best balance between precision and recall

✅ **Random Forest outperformed other models** in detecting high-income individuals, especially in recall and overall F1-score.

---

## 📈 Visualizations Included

- Class distribution bar plot
- Correlation heatmap
- Feature histograms
- Confusion matrices for all models

---

## 🛠 Tools & Technologies

- Python (Jupyter Notebook / Colab)
- Pandas, NumPy
- Scikit-learn (models + metrics)
- Matplotlib, Seaborn

---

## 💡 Future Enhancements

- Use SMOTE or class weights to fix income imbalance
- Hyperparameter tuning with `GridSearchCV`
- Try XGBoost or LightGBM
- Deploy model using Streamlit for live predictions

---

## 🙋‍♀️ About Me

**Wazifa Kapdi**  
Certified Data Science & AI Enthusiast  
📫 [wazifakapde39@gmail.com](mailto:wazifakapde39@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/wazifa-kapdi)  
🔗 [GitHub](https://github.com/Wazifak)  
🔗 [Portfolio](https://datascienceportfol.io/wazifakapde39)

---
