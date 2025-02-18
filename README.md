# Credit Card Fraud Detection

## <h1 style="color:purple">Credit Card Fraud Detection Using Machine Learning</h1>

This repository contains a Python script that implements a **Machine Learning** model to detect fraudulent credit card transactions based on anonymized features.

The dataset used is publicly available and contains credit card transaction data with a binary classification target variable indicating whether the transaction is fraudulent or not.

### Dataset Overview

The dataset consists of the following columns:

- **Time**: The time in seconds from the first transaction.
- **V1 to V28**: Anonymized features generated from the raw data, representing various transformations and statistical metrics.
- **Amount**: The monetary value of the transaction.
- **Class**: A binary target variable indicating whether the transaction is:
  - **0**: Non-fraudulent transaction
  - **1**: Fraudulent transaction

### Approach to Fraud Detection

In this project, we build a machine learning model that can predict fraudulent transactions based on the dataset's features. The steps include:

1. **Data Preprocessing**: Handling missing values, feature scaling, and splitting the data into training and testing sets.
2. **Modeling**: Using **Random Forest Classifier** for detecting fraudulent transactions.
3. **Evaluation**: Evaluating the model using metrics like:
   - **Accuracy**
   - **Precision**
   - **Recall**
   - **F1-Score**
   - **ROC-AUC**

### Model Overview

1. **Training**: A **Random Forest Classifier** is trained on the processed data to learn patterns in fraudulent vs. non-fraudulent transactions.
2. **Evaluation**: Model performance is assessed using metrics like confusion matrix and ROC-AUC score, which are essential for evaluating the effectiveness of fraud detection.
3. **Model Saving**: The trained model is saved for future use and deployment.

### Files in This Repository

- **fraud_detection.py**: Contains the code for data loading, preprocessing, model building, and evaluation.
- **README.md**: The documentation for the project (this file).
  
### How to Run

1. Clone this repository:

    ```bash
    git clone https://github.com/parhamakhand/credit-card-fraud-detection.git
    ```

2. Navigate to the project directory:

    ```bash
    cd credit-card-fraud-detection
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Run the Python script:

    ```bash
    python fraud_detection.py
    ```

The script will process the dataset, train the machine learning model, and output the evaluation metrics.

### Dependencies

Make sure you have the following dependencies installed:

- **pandas**
- **numpy**
- **scikit-learn**
- **matplotlib**
- **seaborn**
- **joblib** (for saving and loading models)

Install them using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib
