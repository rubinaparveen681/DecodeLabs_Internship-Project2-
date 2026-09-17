# Data Science Project 2 — Fraud Detection Pipeline

## Objective
Build a supervised-learning fraud detection pipeline for a highly imbalanced credit-card transaction dataset.

## Requirements covered
- Data inspection and cleaning
- Exploratory Data Analysis
- Train/test split with stratification
- SMOTE for class imbalance
- Logistic Regression
- Random Forest
- Hyperparameter tuning with GridSearchCV
- Precision
- Recall
- ROC-AUC
- Confusion matrices
- ROC curves
- Random Forest feature importance

## Dataset
Credit Card Fraud Detection dataset. The supplied CSV is `creditcard.csv`.

**Important GitHub note:** the dataset file is about 151 MB and therefore should not be committed to normal GitHub storage because GitHub blocks files over 100 MB. Put the CSV in `data/` locally, or use Git LFS if your instructor specifically requires the dataset in the repository.

## Folder structure
```text
Fraud_Detection_Project_2/
├── data/
│   └── creditcard.csv          # place dataset here locally; not included in GitHub ZIP
├── notebooks/
│   └── Fraud_Detection_Project_2.ipynb
├── reports/
│   └── PROJECT_REPORT.md
├── results/
├── src/
├── .gitignore
├── requirements.txt
└── README.md
```

## How to run
1. Install Python 3.
2. Open Jupyter Notebook or JupyterLab.
3. Put `creditcard.csv` inside the `data` folder.
4. Open `notebooks/Fraud_Detection_Project_2.ipynb`.
5. Run cells from top to bottom.

## Important methodology
SMOTE is performed only on training data inside an `imblearn` pipeline. The test set remains untouched so the final Precision, Recall, and ROC-AUC provide an honest evaluation.

## Models
### Logistic Regression
A linear classification model that estimates the probability of fraud.

### Random Forest
An ensemble of decision trees capable of learning non-linear patterns.

## Evaluation
The project brief specifically emphasizes Precision, Recall and ROC-AUC rather than Accuracy. This is appropriate because fraud is a very small minority class.

## Reproducibility
Random seed: `42`.
