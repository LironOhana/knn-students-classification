# KNN Students Classification (Classic ML)

## Overview
A classic machine learning workflow using a K-Nearest Neighbors (KNN) classifier on a small tabular dataset.
Includes EDA, preprocessing, leakage handling, hyperparameter tuning (GridSearchCV), and an optional PCA experiment.

## Dataset
- File: `data/students_data.csv`
- Features: `feature1..feature4`
- Target: `label` (binary)

## Key points
- Identified and removed a leakage feature (`feature4`) due to near-perfect correlation with the label.
- Handled outliers in selected features to reduce bias.
- Applied standardization correctly: fit on train only, transform on validation/test.

## Project structure
```
.
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── students_data.csv
├── notebooks/
│   └── knn_students_classification.ipynb
└── report/
    └── report_redacted.pdf
```

## Run
You can open the notebook on GitHub to view code and outputs, or run it online via Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LironOhana/knn-students-classification/blob/main/notebooks/knn_students_classification.ipynb)

Local setup (optional):
```bash
pip install -r requirements.txt
jupyter notebook

