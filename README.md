# Stroke Prediction Using Logistic Regression

## Project overview
This educational machine-learning project uses the `healthcare-dataset-stroke-data.csv` dataset to train a Logistic Regression model to classify the recorded stroke outcome (`stroke`: 0 = no stroke, 1 = stroke).

The notebook covers:
- Loading and exploring the dataset
- Checking missing values and class imbalance
- Removing the identifier column from model features
- Splitting data into stratified training and testing sets
- Imputing missing values, scaling numeric features, and encoding categorical features
- Training a class-weighted Logistic Regression model
- Evaluating the model with accuracy, precision, recall, F1-score, ROC-AUC, average precision, a classification report, and plots

## Dataset
The CSV file included in this repository is `healthcare-dataset-stroke-data.csv`. It contains patient-related fields such as age, hypertension, heart disease, average glucose level, BMI, smoking status, and the recorded stroke outcome.

The dataset contains missing values in the BMI column and an imbalanced target class distribution. The notebook handles missing values through a preprocessing pipeline and uses `class_weight="balanced"` for the Logistic Regression classifier.

## Requirements
- Python 3.9 or later
- Packages listed in `requirements.txt`

## How to run
1. Download or clone this repository.
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open `stroke_prediction_logistic_regression.ipynb`.
5. Run the notebook cells from top to bottom. Keep the CSV file in the same folder as the notebook.

## Files
- `stroke_prediction_logistic_regression.ipynb` — complete notebook with code and saved outputs
- `healthcare-dataset-stroke-data.csv` — dataset used by the notebook
- `requirements.txt` — Python dependencies

## Limitations and responsible use
This is an educational demonstration, not a clinically validated medical tool. It must not be used to diagnose stroke, make treatment decisions, or replace professional medical care. Class imbalance, dataset quality, possible bias, and the limitations of Logistic Regression can affect model performance and its ability to detect stroke cases.
