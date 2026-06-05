# Diabetes Prediction

This project explores a machine learning workflow for predicting whether a patient is likely to have diabetes based on diagnostic health measurements. It uses the included `diabetes.csv` dataset and walks through data exploration, preprocessing, feature engineering, model training, and model evaluation in a Jupyter notebook.

> This project is for learning and experimentation only. It should not be used for medical diagnosis or clinical decision-making.

## Dataset

The dataset contains numeric health-related features and a binary target column:

- `Pregnancies`
- `Glucose`
- `BloodPressure`
- `SkinThickness`
- `Insulin`
- `BMI`
- `DiabetesPedigreeFunction`
- `Age`
- `Outcome` - target variable where `0` means non-diabetic and `1` means diabetic

## Project Workflow

The notebook follows a complete machine learning pipeline:

1. Problem understanding
2. Exploratory data analysis
3. Univariate, bivariate, and multivariate visualizations
4. Missing-value handling by replacing invalid zero values
5. Feature scaling examples using Min-Max scaling and standardization
6. Train/test split
7. Model training with logistic regression and decision tree classifiers
8. Model evaluation using accuracy, cross-validation, confusion matrix, ROC curve, AUC, and feature importance plots

## Repository Structure

```text
.
├── diabetes.csv
├── fearue_engineering_project.ipynb
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KHALIDKARROUM/Diabetes-Prediction-.git
cd Diabetes-Prediction-
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

```bash
# Windows
.venv\Scripts\activate

# macOS/Linux
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Open the notebook

```bash
jupyter notebook fearue_engineering_project.ipynb
```

Run the cells from top to bottom to reproduce the analysis and model results.

## Model Results

The notebook reports the following results:

| Model | Test Accuracy | Notes |
| --- | ---: | --- |
| Logistic Regression | 0.7532 | AUC-ROC: 0.7961 |
| Decision Tree | 0.7727 | Max depth: 3 |

These results may vary slightly depending on environment, library versions, and notebook execution order.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Future Improvements

- Add a `requirements.txt` file for easier dependency installation
- Compare more models such as random forest, SVM, KNN, or gradient boosting
- Improve feature selection and preprocessing with a Scikit-learn pipeline
- Add hyperparameter tuning
- Export the best model for reuse
- Build a simple prediction web app using Streamlit or Flask
