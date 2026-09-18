# Hospital Readmission Prediction using Logistic Regression (L2)

## Overview

This project predicts whether a patient will be **readmitted within 30 days** after hospital discharge using **Logistic Regression with L2 Regularization**. The model is trained on patient records containing diagnosis information, vital signs, and previous hospital visits.

## Objective

* Predict 30-day hospital readmission risk
* Apply Logistic Regression with **L2 Regularization**
* Evaluate model performance using **ROC-AUC**
* Analyze the clinical impact of **False Negatives** and **False Positives**

## Dataset

**File:** `hospital_readmissions_30k.csv`

The dataset contains approximately **30,000 patient records** with features such as:

* Diagnosis codes
* Vital signs
* Previous hospital visits
* Demographic information
* Target: `readmitted_30_days` (Yes/No)

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

## Machine Learning Workflow

1. Load and inspect the dataset
2. Handle missing values
3. Remove `patient_id`
4. Encode categorical features using One-Hot Encoding
5. Split data into training and testing sets (80:20)
6. Train Logistic Regression with **L2 Regularization**
7. Evaluate using Accuracy, Confusion Matrix, Classification Report, and ROC-AUC
8. Plot the ROC Curve

## Evaluation Metrics

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-Score
* ROC-AUC Score

## Clinical Interpretation

### False Negative (FN)

A patient is predicted as **low risk** but is actually readmitted.

**Clinical Cost:** High, because the patient may miss timely follow-up care, leading to complications and emergency readmission.

### False Positive (FP)

A patient is predicted as **high risk** but is not readmitted.

**Clinical Cost:** Moderate, because it may result in unnecessary monitoring and additional healthcare costs.

> In healthcare, **False Negatives are generally more critical than False Positives**.

## Repository Structure

```text
Hospital-Readmission-Prediction/
│── hospital_readmission_prediction.ipynb
│── hospital_readmissions_30k.csv
└── README.md
```

## How to Run

1. Clone the repository
2. Install the required libraries
3. Open the Jupyter Notebook
4. Run all cells sequentially

## Author

**Syed Ali Raza**

B.Tech CSE (AI & ML)
