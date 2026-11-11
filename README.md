# **Forest Cover Type Prediction**

Author: Claudio W.  
Date: 22.12.2024

---
###  **Overview**

This repository contains my **machine learning classification** pipeline developed as a coursework a couple of years ago. It includes Eplorative data analysis, feature engineering, hyperparameter tuning, and model evaluation. The work is implemented as a single (way to large) Jupyter notebook.

The goal is to classify the dominant forest cover type in a region using features such as elevation, slope, aspect, hydrological distances, soil type indicators, and wilderness area indicators. The target variable is `Cover_Type`, which contains seven classes of forest cover.

---
### **Dataset**

The project uses the *Forest Cover Type Prediction* dataset found on kaggle:
https://www.kaggle.com/competitions/forest-cover-type-prediction/overview

With the training data stored in `data/train.csv` and test set stored in `data/test.csv`.

Key characteristics:
- Multi-class classification problem
- 7 cover-type classes
- Numerical and one-hot encoded land- and soil-related features
- Features include elevation, aspect, slope, hydrology distance measures, road distance, hillshade, wilderness area indicators, and soil-type indicators

---
### **Included work**

The notebook covers:
- Data loading and inspection
- Missing-value and duplicate checks
- Descriptive statistics and distribution analysis
- Feature importance exploration
- Feature engineering (creation of new features)
- Model comparison and hyperparameter tuning using Optuna
- Accuracy evaluation and savings of experiment results

---
### **Repository structure**

- `Forest-Cover-Type_CW.ipynb` — main notebook containing the full workflow
- `data/` — training and test CSV files
- `results/` — CSV exports from model benchmarking and tuning runs
- `assets/` — sketches explaining newly created features
- `requirements.txt` — Python package dependencies
- `db.sqlite3` — Optuna study database used to save hyperparameter optimization results

---
### **Reproducibility of the analysis**

1. Create virtual environment using the requirements.txt file
2. Download optuna extension from vs-code marketplace
3. Run jupyter notebook cells step-by-step
4. Inspect optuna database results by right clicking on database and clicking *Open in Optuna Dashboard*

### **Notes**

The project was done a rather long time ago thus much more experience has been gained and many things would no be done differently.  
Nonetheless is is a nice project displaying the core of modern machine learning workflows. 