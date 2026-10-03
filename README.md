# QuickCart Warehouse Inventory Stockout Risk

## Project Overview

This project focuses on predicting warehouse inventory stockout risk using historical inventory, SKU, store, supplier and event data.

The target variable has three classes:

* Safe
* At-Risk
* Imminent

## Work Done

* Data loading and validation
* Missing-value analysis
* Data cleaning
* Feature engineering
* Supplier reliability handling
* Time-based train/test split
* Majority-class baseline
* Logistic Regression
* Random Forest
* Model evaluation
* Confusion matrix
* Feature importance analysis

## Features Created

* `reorder_gap`
* `days_of_cover_ratio`
* `day_of_month`
* `days_since_festival_start`
* `recent_reorder`
* `reliability_clean`

## Train/Test Split

* Training period: October 1–23, 2026
* Testing period: October 24–30, 2026

## Model Results

| Model               | Accuracy | Balanced Accuracy | Imminent Recall |
| ------------------- | -------: | ----------------: | --------------: |
| Majority Baseline   |   62.28% |            33.33% |           0.00% |
| Logistic Regression |   72.08% |            55.37% |          43.23% |
| Random Forest       |   83.29% |            72.06% |          62.97% |

## Key Finding

The Random Forest model achieved 83.29% accuracy and 62.97% recall for the Imminent stockout-risk class on the test period.

The most important features in the Random Forest model were `days_of_cover_ratio` and `reorder_gap`, followed by `day_of_month`, `recent_reorder`, and `reliability_clean`.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab

## Files

* `QuickCart_Warehouse_Inventory_Stockout_Risk.ipynb` — Complete project notebook
* `README.md` — Project documentation
