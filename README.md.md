# Heart Disease Prediction

A machine learning project for predicting the presence of heart disease using patient health attributes. The project is implemented in Python using a Jupyter Notebook and applies Logistic Regression for binary classification.

## Project Overview

This project performs basic data analysis, visualization, preprocessing, model training, and evaluation on a heart disease dataset.

The target variable is:

- `0` = No heart disease
- `1` = Heart disease present

## Project Files

```text
heart_disease_assignment/
│
├── heart.csv
├── heart_disease.ipynb
├── Heart_Disease_Prediction.pptx
├── literature review and research gap.docx
├── README.md
├── requirements.txt
└── .gitignore
```

## Dataset

The dataset contains 1,025 records and 14 columns.

### Features

- `age` - Age of the patient
- `sex` - Sex
- `cp` - Chest pain type
- `trestbps` - Resting blood pressure
- `chol` - Serum cholesterol
- `fbs` - Fasting blood sugar
- `restecg` - Resting ECG result
- `thalach` - Maximum heart rate achieved
- `exang` - Exercise-induced angina
- `oldpeak` - ST depression induced by exercise
- `slope` - Slope of the peak exercise ST segment
- `ca` - Number of major vessels
- `thal` - Thalassemia-related feature
- `target` - Heart disease prediction label

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Machine Learning Model

The project uses:

```text
Logistic Regression
```

The model is trained using an 80/20 train-test split.

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

The Logistic Regression model is created with:

```python
LogisticRegression(max_iter=1000)
```

## Project Workflow

1. Import required Python libraries
2. Load the `heart.csv` dataset
3. Inspect dataset information
4. Check for missing values
5. Visualize the target classes
6. Separate input features and target variable
7. Split the data into training and testing sets
8. Train a Logistic Regression model
9. Make predictions on test data
10. Evaluate model accuracy

## Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd heart_disease_assignment
```

Or download the repository as a ZIP file and extract it.

### 2. Install the required Python packages

```bash
pip install -r requirements.txt
```

## How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
heart_disease.ipynb
```

Run the notebook cells from top to bottom.

You can also use JupyterLab:

```bash
jupyter lab
```

## Visualization

The notebook includes a count plot for the `target` column to show the distribution of patients with and without heart disease.

## Model Evaluation

The trained Logistic Regression model makes predictions on the test dataset, and performance is evaluated using accuracy:

```python
accuracy_score(y_test, predictions)
```

## Additional Project Documents

The repository also includes:

- `Heart_Disease_Prediction.pptx` - Project presentation
- `literature review and research gap.docx` - Literature review and research-gap document

## Purpose

This project demonstrates the basic machine learning workflow for a healthcare classification problem, including exploratory analysis, preprocessing, model training, prediction, and evaluation.

## Disclaimer

This project is for educational purposes only. It is not intended for medical diagnosis or clinical decision-making.
