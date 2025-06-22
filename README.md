# Machine Learning Project Repository

## Overview

This repository contains a collection of machine learning projects and assignments covering various algorithms and techniques. The projects include implementations of K-Nearest Neighbors (KNN), Regression Models, Support Vector Machines (SVM), and Neural Networks (NN), along with datasets for practice and experimentation.

## Technology Used

- **Programming Language**: Python
- **Libraries**:
  - Scikit-learn (for ML models)
  - Pandas (for data manipulation)
  - NumPy (for numerical operations)
  - Matplotlib/Seaborn (for visualization)
- **Tools**:
  - Jupyter Notebook (for interactive coding)
  - Git (for version control)

## How to Use and Run

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd FULL-PROJECT
2. **Install Dependencies**:

    Ensure you have Python installed (recommended: `Python 3.9`). Install the required libraries using:

    ```bash
    pip install -r requirements.txt
3. **Run Jupyter Notebooks**:

    Navigate to the `notebooks` folder and launch Jupyter:

    ```bash
    jupyter notebook

- Open the desired notebook (e.g., `KNN-Model.ipynb`) and execute the cells to run the code.

4. **Datasets**:

    The `data` folder contains datasets (e.g., `Iris.csv`, `Titanic.csv`). Ensure the notebook paths to these datasets are correctly set.

## Folder Structure

```txt
📦Full-Project
 ┣ 📂data
 ┃ ┣ 📜CarPricePrediction.csv
 ┃ ┣ 📜Iris.csv
 ┃ ┗ 📜Titanic.csv
 ┣ 📂notebooks
 ┃ ┣ 📂KNN-CrossValidation
 ┃ ┃ ┣ 📜KNN-Model.ipynb
 ┃ ┃ ┗ 📜README.md
 ┃ ┣ 📂RegressionModels
 ┃ ┃ ┣ 📜README.md
 ┃ ┃ ┗ 📜RegressionModels.ipynb
 ┃ ┗ 📂SVM-NN Models
 ┃ ┃ ┣ 📜README.md
 ┃ ┃ ┗ 📜SVM-NN-Models.ipynb
 ┣ 📜README.md
 ┗ 📜requirements.txt
```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.

2. Create a new branch for your feature/fix:

   ```bash
   git checkout -b feature-name

3. Commit your changes and push to the branch.

4. Open a Pull Request with a clear description of your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/MidoHossam14/MachineLearningAlgorithms/blob/master/LICENSE) file for details.
