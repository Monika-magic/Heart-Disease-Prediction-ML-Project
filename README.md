
# Heart Disease Prediction Using Machine Learning

A Python-based machine learning project that predicts the presence of heart disease from patient health, lifestyle and clinical features using Logistic Regression.

## Project Overview

This project implements a binary classification model using a dataset of **50,000 patient records**. It covers data inspection, preprocessing, categorical encoding, model training, accuracy evaluation, and sample prediction.

- **Algorithm:** Logistic Regression
- **Dataset:** 50,000 records
- **Input features:** 24 columns before removing the patient identifier
- **Target variable:** `Heart_Disease`
- **Training/testing split:** 80% / 20%
- **Environment:** Google Colab

## Project Notebook

[![Open in Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Monika-magic/Heart-Disease-Prediction-ML-Project/blob/main/Heart_Disease_Prediction.ipynb)

## Features Used

The dataset includes:

- Demographic details: age, sex, height, weight, and BMI
- Lifestyle factors: smoking, physical activity, stress level, and sleep duration
- Medical history: family history, diabetes, and hypertension
- Clinical measurements: blood pressure, cholesterol, HDL, LDL, triglycerides, and fasting glucose
- Cardiac indicators: resting heart rate, maximum heart rate, chest pain type, exercise-induced angina, and resting ECG

The `Patient_ID` column is excluded from model training because it is an identifier rather than a meaningful predictive feature.

## Workflow

1. Load the dataset using Pandas.
2. Inspect dataset dimensions, data types, descriptive statistics, and missing values.
3. Examine the distribution of the target variable.
4. Separate input features and the target.
5. Split the dataset into training and testing sets using stratified sampling.
6. Encode categorical variables using one-hot encoding.
7. Train a Logistic Regression classifier.
8. Evaluate training and test accuracy.
9. Generate a prediction for a sample patient record.

## Model Performance

| Metric | Result |
|---|---:|
| Training accuracy | 74.525% |
| Test accuracy | 74.88% |
| Training records | 40,000 |
| Test records | 10,000 |

These results describe the model's performance on the dataset used in this experiment. Accuracy alone does not establish clinical usefulness or reliability.

## Technologies

- Python
- NumPy
- Pandas
- Scikit-learn
- Google Colab

## How to Run

1. Open the notebook using the Google Colab badge above.
2. Upload `heart_disease_prediction_50000.csv` to the Colab runtime.
3. Ensure the CSV is available at `/content/heart_disease_prediction_50000.csv`, as referenced in the notebook.
4. Run the notebook cells in sequence.

**Note:** The dataset CSV must be provided separately because it is not currently included in the repository.

## Future Improvements

- Resolve the Logistic Regression convergence warning through feature scaling and suitable solver settings.
- Evaluate the model using a confusion matrix, precision, recall, F1-score, and ROC-AUC.
- Implement a consistent preprocessing pipeline for training and inference.
- Validate the model on appropriate, representative data.

## Disclaimer

This project is intended for educational purposes only. It is not a medical diagnostic tool and must not be used to make medical decisions.

---

**Author:** [Monika Sankar](https://github.com/Monika-magic)
