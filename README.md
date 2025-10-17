# Egypt_Estate_Analysis
Exploratory and predictive analysis of Egyptian real estate listings using correlation–regression modeling.
by Adil Rakhimbekov


## Project Overview

1. **Data Preprocessing**
   - Extracted city names from unstructured location data.  
   - Removed invalid and extreme values.  
   - Converted textual fields (`price`, `size`, `bedrooms`) into numeric form.  

2. **Modeling**
   - Polynomial **Ridge Regression (degree = 3)** for nonlinear relationships.  
   - Train/test split for validation.  
   - Evaluation using **R²** and **MSE** metrics.  

3. **Prediction**
   - The model predicts housing price based on user input: city, size, and number of bedrooms.  

4. **Visualization**
   - Scatterplot with fitted regression curve.  
   - Average prices per city.  
   - Density plots for `price` vs. `size` and `bedrooms`.

## Example Workflow:

Notebooks are divided into 3 sections: data preprocessing; correlation-regression prognose by Ridge; # some visualization (might take some time)

Open the notebook in Jupyter and run all cells step by step:

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

