# Breast Cancer Prediction App

This is a web application for predicting breast cancer using a Machine Learning model. The app is built using Streamlit and leverages a pre-trained Artificial Neural Network (ANN) model.

## Overview

The app allows users to input various features of a breast cancer tumor and predicts whether the tumor is malignant or benign. The model used in this app was trained using the Breast Cancer Wisconsin (Diagnostic) dataset.

## Features

- Input real values for specific tumor features.
- Standardizes the input data using a pre-trained scaler.
- Predicts the class (malignant or benign) using a pre-trained ANN model.
- Displays prediction probabilities.

## Requirements

- Python 3.7+
- Streamlit
- NumPy
- Pandas
- Scikit-learn
- Pickle

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Kumarkyrohit/Breast_cancer_analysis_prediction-end-to-end.git
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure the scaler and model pickle files (`scaler.pkl` and `mlp_model.pkl`) are in the project directory. These files are necessary for standardizing the input data and making predictions.

2. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

3. Open your web browser and navigate to `http://localhost:8501` to use the app.

## How It Works

1. **Load the Scaler and Model**: The app loads a pre-trained scaler and ANN model from pickle files.

2. **Get User Input**: The app provides input fields for the user to enter real values for the following features:
    - Mean Radius
    - Mean Perimeter
    - Mean Area
    - Mean Concavity
    - Mean Concave Points
    - Worst Radius
    - Worst Perimeter
    - Worst Area
    - Worst Concavity
    - Worst Concave Points

3. **Standardize Input Data**: The user inputs are standardized using the pre-trained scaler.

4. **Make Prediction**: The standardized data is fed into the pre-trained ANN model to predict whether the tumor is malignant or benign. The prediction probabilities are also displayed.

