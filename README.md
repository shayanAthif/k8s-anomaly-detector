# Kubernetes Failure Prediction and Anomaly Detection

This repository contains a project dedicated to predicting failures and detecting anomalies in Kubernetes clusters using machine learning. It includes data preprocessing, model training with various ML algorithms, and an advanced analysis pipeline for deriving anomalies from the original dataset.

## File Structure

```
.
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
```

## Requirements

- **Python 3.x**
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `xgboost`
  - `tensorflow` (if using deep learning models)
  - `matplotlib`
  - `seaborn`

## How to Use

1. **Preprocessing**

   - Open and run **`K8_preprocessing.ipynb`**.  
   - This notebook loads the dataset, cleans and preprocesses time-related columns, engineers additional features (including derived metrics and failure flags), and detects/normalizes anomalies.

2. **Model Training**

   - Open and run **`K8_model_training&evaluation-1.ipynb`**.  
   - This notebook trains multiple machine learning models (e.g., Logistic Regression, Random Forest, Decision Tree, XGBoost) on the preprocessed data.  
   - It also evaluates the models and saves the best-performing ones in the `models` folder.

3. **Advanced Anomaly Detection**

   - Open and run **`K8_model_training&evaluation-11.ipynb`**.  
   - This notebook derives anomaly-specific features from the original dataset.  
   - It then trains a model specifically for anomaly prediction based on these derived features.

---

Feel free to adjust any file or notebook names to match your exact workflow.
