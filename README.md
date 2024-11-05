# Machine_Learning_Models
Model Scripts created in Python Jupyter's Lab
Code produced by Ayden McCarthy
Manuscript Title: "Machine Learning Models Predict Assessment Outcomes 
                   From Military Physical Employment Standards Via a 
                   Physical Test Battery"
Program of Study: PhD Candidacy
Institution: Macquarie University
Year: 2024
# Model Suite

This repository contains four Jupyter Notebook models developed as part of a scientific manuscript, each designed to predict specific performance metrics using Ridge regression, support vector regression, random forest, and multilayer perceptron models. Each notebook follows a logical order and structure, providing reproducible and transparent data analysis for researchers and practitioners. This suite supports applications in performance modeling, prediction, and cross-validation for various populations.

## Table of Contents

- [Installation](#installation)
- [Models](#models)
  - [Notebook Structure](#notebook-structure)
- [Usage](#usage)
  - [Running the Notebooks](#running-the-notebooks)
  - [Parameter Tuning](#parameter-tuning)
  - [Cross-validation](#cross-validation)
- [Output Files](#output-files)
- [Contributions](#contributions)
- [License](#license)

## Installation

To get started, clone this repository and install the required Python packages. Ensure that you have Python 3 installed and JupyterLab set up. Use the following commands:

```bash
git clone https://github.com/AydenMQ/Machine_Learning_Models.git
cd Machine_Learning_Models
pip install -r requirements.txt
```

Create a `requirements.txt` file with the following content:

```text
pandas==2.2.2
numpy==1.26.4
seaborn==0.12.2
matplotlib==3.8.3
shap==0.43.0
mlxtend==0.23.1
scipy==1.13.0
scikit-learn==1.4.2
```

This ensures compatibility with the specific package versions used in your notebooks.

## Models

This repository includes four Ridge regression models, each in a separate Jupyter Notebook (.ipynb). The models were developed for robust predictive modeling. Each notebook handles data pre-processing, training, hyperparameter tuning, and output generation.

### Notebook Structure

Each model notebook follows the same logical flow:

1. **Data Import**: Load the dataset, which may contain performance metrics, demographic variables, or other features.
2. **Pre-processing**: Handle missing values, feature scaling, and data partitioning into training and test sets.
3. **Model Training**: Train the specified model with tuned hyperparameters.
4. **Validation**: Cross-validation (if applicable) to validate the model's performance and generalization capabilities.
5. **Results Output**: Save the results, including RMSE, and other relevant metrics, to CSV or JSON for reporting.

## Usage

### Running the Notebooks

Open each notebook in JupyterLab and run the cells sequentially. Each cell contains code blocks that need to be executed in order to train and evaluate the model.

1. Start JupyterLab:

   ```bash
   jupyter lab
   ```

2. Open the desired notebook (e.g., `Ridge_Model.ipynb`), and run all cells or step through cells to review intermediate results.

### Parameter Tuning

Each model can be tuned for optimal performance using scikit-learn’s GridSearchCV or manual adjustment within the notebook. Refer to the hyperparameters section to adjust parameters such as `alpha` for Ridge regularization.

### Cross-validation

Cross-validation is incorporated in each notebook to ensure model robustness on unseen data (testing phase). Results include cross-validated RMSE for consistent performance evaluation.

## Output Files

The notebooks generate output files that include:

- **SHAP**: Shows what features are the most influential in reducing the error.
- **Performance Metrics**: Metrics such as RMSE.
- **Prediction Outputs**: Predicted vs. actual performance values for the test dataset.

## Contributions

Contributions are welcome. If you have suggestions for model improvements, feature requests, or bug fixes, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
