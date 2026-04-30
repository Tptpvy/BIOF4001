# 🩺 Sepsis and Coagulation Dysfunction Prediction Using Electronic Health Records

## 📋 Overview

This repository contains the complete data processing pipeline, epidemiological analysis, and machine learning model development for predicting **coagulation dysfunction (CD)** in sepsis patients using electronic health record (EHR) data from Hong Kong's Clinical Data Analysis and Reporting System (CDARS). Data is filtered according to Centers for Disease Control and Prevention (CDC) surveillance criteria, slightly modified to comply with CDARS data.

The project bridges a critical research gap in Hong Kong sepsis epidemiology by providing longitudinal insights over a 22-year period (2003–2025) and develops an experimental machine learning model for early CD risk prediction.

## 📁 Repository Structure

| File/Folder | Description |
|:------------|:------------|
| `ase_filter.ipynb` | 🔍 Filter Adult Sepsis Event (ASE) patients |
| `baseline_table.ipynb` | 📊 Baseline demographic table generation |
| `data_analysis.ipynb` | 📈 Exploratory data analysis scripts |
| `data_preprocessing.ipynb` | 🧹 Data cleaning and handling scripts |
| `model.ipynb` | 🤖 ML model training and feature selection |
| `single_filter.ipynb` | 🩺 Filter presumed infection patients |
| `xls_trans_csv.ipynb` | 🔧 Utility functions (e.g., file conversion) |
| `data_analysis/` | 📉 Data analysis plots and summaries |
| `model/data/` | 🗃️ De-identified data for model development |

## 📦 Requirements

The code is written in **Python 3.11.9** and requires the following packages:

### Core Dependencies

| Package | Version | Purpose |
|:--------|:--------|:--------|
| pandas | ≥1.4.0 | 🐼 Data manipulation and analysis |
| numpy | ≥1.21.0 | 🔢 Numerical computing |
| matplotlib | ≥3.5.0 | 📊 Data visualization |

### Machine Learning Dependencies

| Package | Version | Purpose |
|:--------|:--------|:--------|
| scikit-learn | ≥1.0.0 | 🧠 Model training, CV, preprocessing |
| lightgbm | ≥3.3.0 | 🌳 Gradient boosting model |
| xgboost | ≥1.5.0 | 🚀 Gradient boosting model |
| imbalanced-learn | ≥0.9.0 | ⚖️ SMOTE-NC for class imbalance |
| shap | ≥0.40.0 | 🔍 Model interpretability |

### Utility Dependencies

| Package | Version | Purpose |
|:--------|:--------|:--------|
| openpyxl | ≥3.0.0 | 📑 Excel file handling |
| scipy | ≥1.7.0 | 📐 Statistical tests |

### Installation

```bash
# Clone the repository
git clone https://github.com/Tptpvy/BIOF4001.git
cd BIOF4001
```

### ⚖️ License
The source code in this repository is released under the MIT License. The CDARS data used in this study is proprietary to the Hong Kong Hospital Authority and is not included in this repository. This work is for academic research purposes only.
