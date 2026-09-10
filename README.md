# Disease Prediction System

A machine learning project that classifies patients into two classes — No Disease (0) and Disease (1) — using the UCI Heart Disease dataset.

## Project Overview

The objective of this project is to build and evaluate classification models using patient health-related features.

The project covers the complete machine learning workflow:

- Data collection
- Data inspection
- Data preprocessing
- Missing value handling
- Exploratory Data Analysis (EDA)
- Feature scaling
- Model training
- Model evaluation
- Model comparison
- Prediction on new data
- Model saving

## Dataset

This project uses the **UCI Heart Disease Dataset**.

- Number of records: 303
- Number of features: 13
- Target variable: Heart disease presence
- Target converted into binary classification:
  - `0` → No Disease
  - `1` → Disease

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Google Colab

## Data Preprocessing

The following preprocessing steps were performed:

1. Checked the dataset structure and data types.
2. Checked for duplicate records.
3. Identified missing values.
4. Handled missing values in the `ca` and `thal` features using median imputation.
5. Converted the original multi-class target into a binary target.
6. Split the dataset into training and testing sets using an 80:20 ratio.
7. Applied StandardScaler to the training and testing features.

## Exploratory Data Analysis

EDA was performed to understand the distribution and relationships within the dataset.

Visualizations included:

- Age distribution
- Heart disease class distribution
- Age distribution by disease class
- Feature correlation matrix

## Machine Learning Models

Two classification algorithms were implemented:

### 1. Logistic Regression

Logistic Regression was used as the primary classification model.

**Accuracy: 86.89%**

### 2. Decision Tree

A Decision Tree classifier was trained and evaluated for comparison.

**Accuracy: 73.77%**

## Model Comparison

| Model | Accuracy |
|---|---:|
| Logistic Regression | 86.89% |
| Decision Tree | 73.77% |

Based on the test-set accuracy obtained in this project, **Logistic Regression performed better** than the Decision Tree.

## Prediction

The trained Logistic Regression model was tested using new sample patient data.

The model can provide:

- Predicted class
- Probability for No Disease
- Probability for Disease

The trained model and feature scaler were saved using Joblib for future reuse.

## Project Structure

```text
Disease-Prediction-System/
│
├── Disease_Prediction_System.ipynb
├── README.md
├── logistic_regression_model.pkl
└── scaler.pkl

## How to Run

1. Open the Jupyter Notebook in Google Colab.
2. Run the cells sequentially.
3. Install the required libraries if necessary.
4. Load and preprocess the dataset.
5. Train the classification models.
6. Evaluate and compare the models.
7. Test the final model with new input data.

## Key Learning Outcomes

Through this project, I practiced:

- Data preprocessing with Pandas
- Exploratory Data Analysis
- Data visualization
- Binary classification
- Train-test splitting
- Feature scaling
- Logistic Regression
- Decision Tree classification
- Model evaluation
- Model comparison
- Saving and reusing ML models

## Disclaimer

This project is developed for **educational and learning purposes only**.

It is not a clinically validated system and should not be used for medical diagnosis, treatment, or real-world clinical decision-making.
