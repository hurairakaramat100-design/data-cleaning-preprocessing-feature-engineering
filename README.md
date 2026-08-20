# Data Cleaning, Preprocessing and Feature Engineering

Two end-to-end notebooks + a written report, covering the full checklist: data-quality auditing,
a deliberately-corrupted dataset for practice, missing-value treatment, categorical encoding,
numerical scaling, feature engineering, data splitting, data leakage, and reusable scikit-learn
Pipelines.

## Datasets
- **Titanic** (`data/titanic_*.csv`) — classification, categorical/mixed-type heavy.
- **California Housing Prices** (`data/housing_*.csv`) — regression, numerically heavy.

Each has `_raw` (original), `_messy` (deliberately corrupted copy), and `_cleaned` (final output).

## Folders
- `notebooks/` — the two fully executed Jupyter notebooks (open with Jupyter, or view the saved
  outputs directly since they were run end-to-end already).
- `data/` — raw, messy, and cleaned CSVs for both datasets.
- `pipelines/` — saved, fitted scikit-learn pipelines (`joblib.load(...)` to reuse).
- `report/Data_Preprocessing_Report.docx` — the written report (Practical Task 7) summarizing
  methodology, comparisons, and results for both datasets.

## Results
- Titanic (Logistic Regression): 80.6% test accuracy.
- Housing (Linear Regression): R² = 0.658, MAE ≈ $48,918 on the test set.
