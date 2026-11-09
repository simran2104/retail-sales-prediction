# 🛒 Retail Sales Prediction Using Machine Learning

A machine learning project to predict product-level retail sales using historical product and store data.

## 📌 Project Overview

The objective of this project is to predict the sales of a particular product at a specific store using product characteristics, pricing and store-related information.

The dataset contains 8,540 records with 14 columns. The project explores sales patterns, prepares the data and compares different regression algorithms to identify a suitable prediction model.

## 🔍 What I Worked On

- **Exploratory Data Analysis:** Analysed sales distributions and relationships between sales, product categories, prices, store types, store sizes and other features.
- **Data Cleaning:** Identified invalid numerical values, handled extreme observations and standardised inconsistent categorical labels.
- **Feature Engineering:** Extracted Product Code and Product ID from the original product identifier.
- **Data Preprocessing:** Applied median and most-frequent imputation, One-Hot Encoding, Ordinal Encoding and StandardScaler.
- **Machine Learning Pipeline:** Built a Scikit-learn pipeline to combine data preprocessing and model training.
- **Model Evaluation:** Compared eight regression models using five-fold cross-validation and evaluated selected models on a separate test dataset.

## 🤖 Models Compared

| Regression Model |
|---|
| Linear Regression |
| Ridge Regression |
| Lasso Regression |
| Elastic Net |
| Bayesian Ridge |
| K-Nearest Neighbours |
| Random Forest |
| Histogram-Based Gradient Boosting |

## 📊 Final Model Results

**Histogram-Based Gradient Boosting** was selected as the final model based on its cross-validation and test performance.

| Evaluation Metric | Test Result |
|---|---:|
| R² Score | **0.6167** |
| MAE | 748.05 |
| RMSE | 1,063.94 |

The model explained approximately 61.67% of the variation in sales in the test dataset.

## 🧰 Technologies Used

- **Language:** Python
- **Data Analysis:** Pandas, NumPy
- **Visualisation:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Environment:** Jupyter Notebook

## 📁 Repository Structure

```text
├── dataset/
│   ├── train.csv
│   ├── test.csv
│   └── readme.md
├── output/
│   └── predicted_sales.csv
├── sales_prediction-model.ipynb
├── requirements.txt
└── README.md
```

## 💡 Key Learnings

- Working with real-world retail data and handling data quality issues.
- Building preprocessing pipelines for numerical and categorical features.
- Comparing linear and tree-based regression algorithms.
- Applying cross-validation and evaluating models using R², MAE and RMSE.
- Understanding how machine learning predictions can support retail sales analysis and inventory planning.
