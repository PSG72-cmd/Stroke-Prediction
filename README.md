# Stroke Prediction: Data Cleaning and Visualization

A Python data cleaning and exploratory analysis project on the Stroke Prediction dataset.

## Team
- PSG72-cmd (Prathmesh Sharma): data cleaning
- kathanmehta926-afk: visualizations

## Dataset
- Source: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
- 5,110 patient records, 12 columns (age, gender, hypertension, heart disease, glucose level, BMI, smoking status, stroke, etc.)
- Goal: find which factors are linked to stroke

## Data cleaning (01_data_cleaning.ipynb)
- Filled missing BMI values with the median
- Checked and removed duplicate rows
- Removed the single row with gender "Other"
- Dropped the `id` column
- Converted 5 text columns to category type
- Capped outliers in BMI and glucose using the IQR method
- Result: 5,109 rows, 11 columns, 0 missing values

## Visualizations (02_visualizations.ipynb)
1. Stroke vs no stroke count: only about 4.9% had a stroke (imbalanced data)
2. Age distribution
3. Age vs stroke: median age 71 (stroke) vs 43 (no stroke)
4. Glucose level vs stroke
5. Hypertension vs stroke rate: 13.3% with vs 4.0% without
6. Smoking status vs stroke
7. Correlation heatmap: age has the strongest link with stroke

## Tools and libraries
Python, Google Colab, pandas, numpy, matplotlib, seaborn, Git/GitHub

## Files
- `healthcare-dataset-stroke-data.csv`: raw data
- `stroke_cleaned.csv`: cleaned data
- `1_...png` to `7_...png`: saved charts
- `01_data_cleaning.ipynb`, `02_visualizations.ipynb`: code notebooks

## How to run
Open each notebook in Google Colab and click Runtime, then Run all.
