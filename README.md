# Kubernetes Failure Prediction and Anomaly Detection

This repository contains a project for predicting failures and detecting anomalies in Kubernetes clusters using machine learning. The project includes data preprocessing, model training with various machine learning algorithms, and an advanced analysis pipeline that derives anomalies from the original dataset.

## File Structure

├── data
│   └── dataset.txt
├── models
│   ├── best_model_final.pkl
│   └── best_model_anomaly.pkl
├── presentation
│   └── Project_Presentation.pptx
└── src
    ├── K8_preprocessing.ipynb
    ├── K8_model_training&evaluation-1.ipynb
    └── K8_model_training&evaluation-11.ipynb

## Requirements

* **Python 3.x**
* Required packages (see `requirements.txt` if available):
  * pandas
  * numpy
  * scikit-learn
  * xgboost
  * tensorflow (if using deep learning models)
  * matplotlib
  * seaborn

## How to Use

1. **Preprocessing:**

   Open and run the `01_Preprocessing.ipynb` notebook. This notebook:

   * Loads the dataset.
   * Cleans and preprocesses time-related columns.
   * Engineers features including derived metrics and failure flags.
   * Detects anomalies and normalizes the data.
2. **Model Training:**

   Open and run the `02_Model_Training.ipynb` notebook. This notebook:

   * Trains various machine learning models (e.g., Logistic Regression, Random Forest, Decision Tree, XGBoost) on the preprocessed data.
   * Evaluates the models and saves the best-performing ones in the **models** folder.
3. **Advanced Anomaly Detection:**

   Open and run the `03_Advanced_Anomaly_Detection.ipynb` notebook. This notebook:

   * Uses the original dataset to derive anomaly-specific features.
   * Trains a model to predict anomalies based on these derived features.
