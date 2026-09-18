# Hospital_readmission_Prediction
# Hospital Readmission Prediction

## 📌 About the Project

This project focuses on predicting whether a patient will be **readmitted to the hospital within 30 days** using Machine Learning.

The project uses **Logistic Regression** and compares its performance **without L2 regularization and with L2 regularization**.

---

## 🎯 Objective

The main objective is to predict the 30-day hospital readmission of a patient based on different patient-related features.

### Target Variable
`readmitted_30days`

- `0` → Not readmitted within 30 days
- `1` → Readmitted within 30 days

---

## 📊 Dataset Features

The dataset contains patient-related information such as:

- Age
- Length of Stay
- Number of Diagnoses
- Number of Medications
- Previous Admissions
- Glucose Level
- BMI
- Diabetes Status
- Discharge Type

---

## 🔧 Technologies Used

- Python
- Pandas
- Scikit-learn
- Logistic Regression
- NumPy
- Google Colab

---

## ⚙️ Methodology

The project follows these steps:

1. Load the dataset
2. Separate features and target variable
3. Identify numerical and categorical features
4. Handle missing values
5. Scale numerical features using `StandardScaler`
6. Encode categorical features using `OneHotEncoder`
7. Split the dataset into training and testing sets
8. Train Logistic Regression without L2 regularization
9. Train Logistic Regression with L2 regularization
10. Predict probabilities
11. Convert probabilities into predictions using a 0.5 threshold
12. Evaluate the models

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression is used because the target variable has two classes:

- `0` → Not readmitted
- `1` → Readmitted

Two models were compared:

- Logistic Regression without L2 regularization
- Logistic Regression with L2 regularization

---

## 📈 Evaluation Metrics

The models were evaluated using:

- ROC-AUC
- Confusion Matrix
- False Negatives
- Classification Report

### ROC-AUC Results

| Model | ROC-AUC |
|---|---:|
| Without L2 | 0.87513 |
| With L2 | 0.87506 |

### False Negatives

| Model | False Negatives |
|---|---:|
| Without L2 | 678 |
| With L2 | 675 |

---

## 📌 Confusion Matrix

### Without L2

```text
[[2584  648]
 [ 678 2550]]
