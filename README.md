# Classification-of-Diabetes-in-Pima-Indians-using-Multiple-Models
Diabetes is a long-term condition impacting countless people around the globe. Identifying issues early and using data analysis can assist in avoiding complications and optimizing treatment management. The aim of this research is to develop a precise prediction model that evaluates whether an individual has diabetes based on various health factors.

## 📊 Dataset Overview
- **Source**: [Kaggle - Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Attributes**: Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age

## 🧪 Models Implemented
- ✅ Logistic Regression
- ✅ Decision Tree
- ✅ Random Forest
- ✅ Stochastic Gradient Descent (SGD)
- ✅ Support Vector Machine (SVM)

## ⚙️ Methodology
1. **Data Preprocessing**: Missing values, outliers, scaling, SMOTE balancing
2. **Training & Evaluation**: 80-20 split, Accuracy, Precision, Recall, F1-Score
3. **Hyperparameter Tuning**: GridSearchCV for each model

## ✅ Results
| Model               | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 81.05%   | 82.22%    | 78.72% | 80.43%   |
| Decision Tree      | 70.83%   | 68.70%    | 70.21% | 69.00%   |
| Random Forest      | 83.16%   | 80.39%    | 87.23% | 83.67%   |
| SGD Classifier     | 75.3%    | 76.1%     | 74.5%  | 75.3%    |
| SVM                | 83.16%   | 81.63%    | 85.11% | 83.33%   |

## 🔍 Key Insights
- **Top Features**: Glucose, BMI, Age
- **Best Overall**: Random Forest & Logistic Regression
- **Best Recall (Less False Negatives)**: SGD Classifier
