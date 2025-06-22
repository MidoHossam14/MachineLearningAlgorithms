# Machine Learning - Assignment 1

This repository contains the notebook **RegressionModels.ipynb**, which demonstrates the application of various regression and classification models on real-world datasets. The assignment covers the following topics:

- Simple and Multiple Linear Regression
- Polynomial Regression
- Logistic Regression (Classification)

## Author

**Mohamed Hossam Darwish**

---

## Datasets Used

- **Car Price Prediction** ([Kaggle Link](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction))  
  File: `1-CarPricePrediction.csv`  
  Used for: Linear Regression (Simple & Multiple), Polynomial Regression

- **Titanic Survival** ([Kaggle Link](https://www.kaggle.com/datasets/heptapod/titanic))  
  File: `2-Titanic.csv`  
  Used for: Logistic Regression (Classification)

---

## Notebook Overview

### 1. Linear Regression (Simple & Multiple)

- **Goal:** Predict car prices using features such as engine size, curb weight, horsepower, etc.
- **Process:**  
  - Data loading and exploratory analysis  
  - Feature selection and preprocessing (encoding, scaling)  
  - Simple Linear Regression using a single feature  
  - Multiple Linear Regression using all relevant features  
  - Evaluation using R² and MSE metrics  
  - Visualization of results

### 2. Polynomial Regression

- **Goal:** Capture non-linear relationships between features and car price.
- **Process:**  
  - Polynomial feature transformation (degrees 2, 3, 4)  
  - Model training and evaluation  
  - Visualization for degree 2

### 3. Logistic Regression (Classification)

- **Goal:** Predict Titanic passenger survival.
- **Process:**  
  - Data loading, cleaning, and exploratory analysis  
  - Handling missing values and encoding categorical variables  
  - Feature scaling  
  - Model training and evaluation (confusion matrix, classification report)  
  - Hyperparameter tuning using GridSearchCV

---

## Key Findings

- **Linear Regression:**  
  - Engine size is a strong predictor of car price.
  - Multiple features improve prediction accuracy.

- **Polynomial Regression:**  
  - Degree-2 polynomial regression balances complexity and performance.
  - Higher degrees may overfit.

- **Logistic Regression:**  
  - Proper preprocessing is essential for classification tasks.
  - The model achieved reasonable accuracy on the Titanic dataset.

---

## Limitations

- Imputation of missing values may introduce bias.
- Further feature engineering could improve classification results.

---

## How to Run

1. Ensure you have Python 3.x and the required libraries:
    - pandas, numpy, matplotlib, seaborn, scikit-learn

2. Place the datasets (`1-CarPricePrediction.csv`, `2-Titanic.csv`) in the same directory as the notebook.

3. Open and run the notebook:  
    [RegressionModels.ipynb](RegressionModels.ipynb)

---

## License

This project is for educational purposes.
