# Lung Cancer Prediction Using Machine Learning

## Overview
This project explores a lung cancer survey dataset and applies multiple machine learning algorithms to analyze factors associated with lung cancer-related symptoms and behaviors. The notebook includes data preprocessing, visualization, feature selection, model training, evaluation, and hyperparameter tuning.

## Dataset
The project uses:

- `survey lung cancer.csv`

The dataset contains demographic, behavioral, and health-related attributes such as:

- Age
- Smoking
- Anxiety
- Yellow Fingers
- Coughing
- Other survey-based health indicators

## Project Workflow

### 1. Data Loading
The dataset is loaded using Pandas.

### 2. Exploratory Data Analysis (EDA)
Performed basic dataset inspection:

- View sample records
- Check dataset shape
- Generate descriptive statistics
- Check for missing values

### 3. Data Visualization
Visualizations include:

- Count plot for **COUGHING**
- Pie chart for **YELLOW_FINGERS**
- Correlation heatmap

Libraries used:

- Matplotlib
- Seaborn

### 4. Data Preprocessing
Preprocessing steps include:

- Min-Max normalization for selected features:
  - SMOKING
  - ANXIETY
  - AGE
- Label encoding of categorical variables
- One-hot encoding where applicable
- Feature scaling using `StandardScaler`

### 5. Feature Selection
Feature selection is performed using:

- `SelectKBest`
- `f_classif`

The selected features are used for model training.

### 6. Model Training
The following machine learning models are trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. Support Vector Machine (SVM)
5. K-Nearest Neighbors (KNN)

### 7. Model Evaluation
Models are evaluated using:

- Accuracy Score
- Classification Report

### 8. Hyperparameter Tuning
Grid Search Cross Validation (`GridSearchCV`) is used for:

- KNN optimization
- SVM optimization
- Decision Tree optimization

## Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Running the Project

1. Open the Jupyter Notebook.
2. Ensure the dataset file is available in the working directory.
3. Run all notebook cells sequentially.

## Project Structure

```text
.
├── Ahmed_Moniem_211001069_machine_learning_lung_cancer.ipynb
├── survey lung cancer.csv
└── README.md
```

## Future Improvements

- Improve feature engineering.
- Add additional evaluation metrics.
- Perform cross-validation for all models.
- Deploy the best-performing model as a web application.
- Experiment with advanced ensemble methods.

## Author

Ahmed Moniem
Student ID: 211001069
