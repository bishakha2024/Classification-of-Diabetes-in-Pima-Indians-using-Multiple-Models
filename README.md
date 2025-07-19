# 🧠 Classification of Diabetes in Pima Indians using Machine Learning

This project was developed as part of the **AASD 4001: Mathematical Concepts for Machine Learning** course under the **School of Computer Technology**.

## 📌 Course Term Project Requirements
As per the project brief:
- ✅ Use a classification dataset with 2+ classes, 5+ features, and 200+ samples.
- ✅ Preprocess and clean the data.
- ✅ Apply the following classifiers:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Stochastic Gradient Descent (SGD)
  - Support Vector Machine (SVM)
- ✅ Use GridSearchCV to tune hyperparameters and observe performance.
- ✅ Randomly or logically remove features and analyze the performance change.
- ✅ Present findings in class (max 15 mins) and submit a technical report (max 15 pages) with Jupyter notebook code.

---

## 📚 Dataset Description

- **Dataset Used**: [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Total Samples**: 768
- **Target Variable**: Diabetes outcome (`0` = No, `1` = Yes)
- **Features**:
  - Pregnancies
  - Glucose
  - BloodPressure
  - SkinThickness
  - Insulin
  - BMI
  - DiabetesPedigreeFunction
  - Age
---

## 🧪 Methodology

### ✅ Data Preprocessing
- Handled missing values using imputation
- Detected and reduced outliers (especially in Insulin and BMI)
- Scaled features and used **SMOTE** for class balancing
- Feature selection using **RFECV**

### ✅ Models Implemented
| Model               | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 81.05%   | 82.22%    | 78.72% | 80.43%   |
| Decision Tree      | 70.83%   | 68.70%    | 70.21% | 69.00%   |
| Random Forest      | 83.16%   | 80.39%    | 87.23% | 83.67%   |
| SGD Classifier     | 75.3%    | 76.1%     | 74.5%  | 75.3%    |
| SVM                | 83.16%   | 81.63%    | 85.11% | 83.33%   |

### ✅ Hyperparameter Tuning (GridSearchCV)
- Tuned parameters for each model
- **SGD** showed the **most improvement in F1 score** (from 0.60 → 0.75)
- Logistic Regression and Random Forest maintained consistent strong performance

### ✅ Feature Removal Impact
- Glucose, BMI, and Age were the **most important** predictors
- Models were re-evaluated after removing low-importance features (like SkinThickness and Insulin)
- Performance of Decision Tree decreased significantly after feature removal

---

## 🧾 Deliverables

- ✅ Final Report: [Report.pdf](./reports/Report.pdf)
- ✅ Jupyter Notebooks: [`/notebooks`](./notebooks)
- ✅ Presentation Slides: [presentation.pptx](./reports/presentation.pptx) 
- ✅ Python Scripts: [`/src`](./src)
- ✅ `README.md`: This file
