# 🚢 Titanic Survival Prediction

## 📌 Project Overview
This project predicts whether a passenger survived the Titanic disaster using Machine Learning.

The goal is to build a complete ML pipeline including preprocessing, feature engineering, model training, and evaluation.

---

## 📂 Dataset
- Dataset: Titanic dataset
- Target variable: `Survived`
- Features include:
  - Age, Fare, Pclass
  - Sex, Embarked
  - SibSp, Parch

---

## ⚙️ Project Workflow

### 🔹 1. Data Preprocessing
- Dropped unnecessary columns:
  - PassengerId, Name, Ticket, Cabin
- Handled missing values using:
  - Median (numerical)
  - Most frequent (categorical)

---

### 🔹 2. Feature Engineering
- Created new features:
  - `FamilySize = SibSp + Parch + 1`
  - `IsAlone = 1 if FamilySize == 1 else 0`

---

### 🔹 3. Pipelines
- Numerical Pipeline:
  - Imputation + Standard Scaling
- Categorical Pipeline:
  - Imputation + One-Hot Encoding
- Combined using ColumnTransformer

---

### 🔹 4. Models Used
- Logistic Regression
- Random Forest Classifier

---

### 🔹 5. Model Evaluation
- Accuracy Score
- ROC-AUC Score
- Cross Validation (5-fold)

---

## 📊 Results

| Model                | Accuracy | ROC-AUC |
|---------------------|----------|--------|
| Logistic Regression | ~0.80    | ~0.85  |
| Random Forest       | ~0.83    | ~0.88  |

---

## 📈 Visualizations
- Histogram plots
- Boxplots
- Countplots
- Correlation Heatmap
- ROC Curve

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
