# Machine Learning - Assignment 2

This repository contains the notebook **KNN-Model.ipynb**, which demonstrates the application of the K-Nearest Neighbors (KNN) algorithm and cross-validation techniques for classification tasks using the Titanic dataset.

## Author

**Mohamed Yasser El-Nafrawy**

---

## Dataset Used

- **Titanic Survival Dataset**  
  File: `Titanic.csv`  
  Source: [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/heptapod/titanic)  
  Used for: Predicting passenger survival using KNN classification

---

## Notebook Overview

### 1. Data Preparation & Preprocessing

- Selected relevant features: `survived`, `pclass`, `sex`, `age`, `fare`
- Encoded categorical variables (e.g., `sex`)
- Handled missing values by dropping incomplete rows
- Split data into training, validation, and test sets for robust evaluation

### 2. KNN Model Selection & Evaluation

- Explored different values of K (neighbors) to find the optimal K using validation accuracy
- Trained the final KNN model with the best K and evaluated on the test set
- Reported metrics: Accuracy, Precision, Recall, F1 Score

### 3. Cross-Validation

- Applied 5-fold cross-validation to assess the model's generalization on the training set

### 4. Visualization & Insights

- Plotted confusion matrix for model performance
- Visualized survival rates by gender, passenger class, age, and fare
- Displayed the correlation matrix for feature relationships

---

## Enhanced Insights

### Survival by Gender

- **Females had a significantly higher survival rate than males.**  
  The countplot shows that the majority of female passengers survived, while most male passengers did not. This reflects the "women and children first" policy during the Titanic disaster.

### Survival by Passenger Class

- **First-class passengers had the highest survival rates, while third-class had the lowest.**  
  The visualization reveals a clear social stratification in survival, with wealthier passengers more likely to survive.

### Age Distribution by Survival

- **Younger passengers, especially children, had a higher chance of survival.**  
  The age distribution plot shows a noticeable peak in survival among children, supporting the prioritization of children during evacuation.

### Fare Distribution by Survival

- **Passengers who paid higher fares were more likely to survive.**  
  The fare distribution plot (for fares < 100) indicates that survival rates increase with fare, again highlighting the advantage of higher socioeconomic status.

### Correlation Matrix

- **Strongest positive correlation:** Fare and survival (higher fare, higher survival probability)
- **Strongest negative correlation:** Male gender and survival (being male reduced survival odds)
- **Class and survival:** Lower class (higher pclass number) is negatively correlated with survival

### Model Performance & Overfitting

- The optimal K was chosen based on validation accuracy, ensuring the model is neither too simple nor too complex.
- Cross-validation and test set results were consistent, indicating **no significant overfitting**.
- The model achieved balanced accuracy, precision, recall, and F1 scores, confirming its reliability.

---

## How to Run

1. Ensure you have Python 3.x and the required libraries:
    - pandas, numpy, matplotlib, seaborn, scikit-learn

2. Place the dataset (`Titanic.csv`) in the same directory as the notebook.

3. Open and run the notebook:  
    [KNN-Model.ipynb](KNN-Model.ipynb)

---

## License

This project is for educational purposes.
