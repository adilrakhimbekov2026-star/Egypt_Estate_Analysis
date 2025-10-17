# Egypt_Estate_Analysis

Exploratory and predictive analysis of Egyptian real estate listings using correlation–regression modeling.  
By Adil Rakhimbekov

## Project overview

This repository contains a small project for cleaning, exploring and predicting housing prices in Egypt using polynomial Ridge regression.
The project was created as part of my process of learning and practicing correlation–regression analysis techniques on real data.

### 1. Data preprocessing
- Extract city names from unstructured `location` text.  
- Remove invalid and extreme values.  
- Convert textual fields (`price`, `size`, `bedrooms`) to numeric types.

### 2. Modeling
- Polynomial **Ridge Regression** (degree = 3) to capture nonlinear effects.  
- Train/test split for validation.  
- Evaluation using **R²** and **MSE**.

### 3. Prediction
- Model predicts price given: **city**, **size (sqm)** and **number of bedrooms**.

### 4. Visualization
- Scatter plot with fitted prediction curve.  
- Average prices per city.  
- Density plots for `price` vs `size` and `bedrooms`.

## Usage

Notebooks are split into three parts: data preprocessing; correlation–regression (Ridge); visualizations.  
Run the preprocessing notebook first, then the modeling and visualization notebooks.

Open and run the notebook in Jupyter:

```bash
jupyter notebook real_estate_analysis.ipynb

# example input
City: Cairo
Size: 120
Bedrooms: 3

# example output
Model for the: Cairo city
R²: 0.23223503765751596
MSE: 14479546581844.588
Price prognose in Cairo: 5,612,812 EGP
```

