# Machine Learning - Assignment 3

This repository contains the notebook **SVM-NN-Models.ipynb**, which demonstrates the implementation, training, and evaluation of Support Vector Machine (SVM) and Neural Network (NN) models on the classic Iris dataset. The notebook includes exploratory data analysis, model comparison, and in-depth insights beyond visualizations.

## Authors

- محمد حسام الدين محمد محمد  
- محمد ياسر محمد سليمان النفراوي  
- محمد أيمن السيد أحمد حامد  

---

## Dataset Used

- **Iris Dataset**  
  Source: [scikit-learn built-in](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html)  
  Features: Sepal length, Sepal width, Petal length, Petal width  
  Target: Species (`setosa`, `versicolor`, `virginica`)

---

## Notebook Overview

### 1. Data Preparation & EDA

- Loaded the Iris dataset and converted it to a DataFrame for easier manipulation.
- Explored the data using pair plots and boxplots to visualize feature distributions and class separability.
- Checked for missing values and standardized features for optimal model performance.

### 2. Support Vector Machine (SVM)

- Trained SVM classifiers with different kernels (`linear`, `poly`, `rbf`).
- Evaluated each model using accuracy and detailed classification reports.
- Selected the best-performing kernel (RBF) based on test accuracy.
- Visualized the confusion matrix for the best SVM model.

### 3. Neural Network (NN)

- Built a feedforward neural network using TensorFlow/Keras with dropout for regularization.
- Used early stopping to prevent overfitting and monitored validation loss.
- Evaluated the NN on the test set with accuracy and classification report.
- Visualized training history (accuracy and loss curves) and confusion matrix.

### 4. Model Comparison & ROC Analysis

- Compared SVM and NN using accuracy, precision, recall, and F1-score.
- Plotted multi-class ROC curves (one-vs-rest) for both models.
- Visualized model accuracy comparison with bar plots.

---

## Insights Beyond Visualizations

### Feature Relationships & Class Separability

- **Petal length and petal width are the most discriminative features** for classifying Iris species, as shown by clear separation in pair plots.
- **Setosa is linearly separable** from the other two classes, while `versicolor` and `virginica` show some overlap, making them harder to distinguish.

### SVM Model Insights

- **RBF kernel outperformed linear and polynomial kernels**, indicating that the decision boundaries between classes are non-linear.
- SVM achieved high accuracy (>97%), with most misclassifications occurring between `versicolor` and `virginica`.
- The confusion matrix confirmed that `setosa` was perfectly classified, while a few samples of `versicolor` and `virginica` were confused with each other.

### Neural Network Model Insights

- The neural network also achieved high accuracy, closely matching SVM performance.
- Training curves showed **good convergence and minimal overfitting** due to early stopping and dropout.
- The NN was able to model complex, non-linear relationships, but did not significantly outperform SVM on this dataset, likely due to the small size and simplicity of Iris.

### Comparative Analysis

- **Both models are highly effective** for the Iris dataset, with SVM (RBF) having a slight edge in accuracy.
- **ROC curves and AUC values** for both models were close to 1.0 for all classes, confirming strong discriminative power.
- **Precision, recall, and F1-scores** were all high, indicating balanced performance across classes.

### Beyond the Plots: Practical Implications

- **Model Selection:** For small, well-behaved datasets like Iris, SVMs are highly competitive and computationally efficient. Neural networks offer flexibility but may not provide significant gains unless the data is more complex.
- **Feature Importance:** The analysis highlights the importance of petal measurements for Iris classification, suggesting that dimensionality reduction or feature selection could further streamline the modeling process.
- **Generalization:** Both models generalized well, as evidenced by consistent validation and test metrics, and the use of early stopping and regularization in NN further ensured robustness.

---

## How to Run

1. Ensure you have Python 3.x and the required libraries:
    - numpy, pandas, matplotlib, seaborn, scikit-learn, tensorflow, keras

2. Open and run the notebook:  
    [SVM-NN-Models.ipynb](SVM-NN-Models.ipynb)

---

## Recommendations & Next Steps

- Experiment with deeper or alternative NN architectures for more complex datasets.
- Tune SVM hyperparameters (C, gamma) for potential further improvements.
- Apply these models to larger, real-world datasets to explore their scalability and performance.
- Investigate feature engineering or dimensionality reduction for enhanced interpretability.

---

## License

This project is for educational purposes.
