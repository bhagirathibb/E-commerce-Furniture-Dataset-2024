# E-commerce Furniture Dataset 2024 Project

## Problem Statement

The objective of this project is to predict the number of furniture items sold based on product attributes such as product title, original price, price, and tag text. The project involves exploratory data analysis, feature engineering, machine learning modeling, and evaluation.

## Dataset Description

This dataset consists of 2000 entries scraped from AliExpress, containing details about furniture products including key sales metrics and product descriptions.

Columns:
- productTitle: Name of the furniture item.
- originalPrice: The original price before any discount.
- price: Current selling price.
- sold: Number of units sold.
- tagText: Additional tags such as "Free shipping".

The data was collected ethically, complying with user privacy and platform terms.

## Tools and Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Workflow

### 1. Data Collection
- Loaded the dataset using pandas from a CSV file.
- Displayed the first few rows to understand structure.

### 2. Data Preprocessing
- Checked and handled missing values.
- Dropped irrelevant or mostly missing columns like originalPrice.
- Cleaned and transformed 'price' column by removing dollar symbols and converting to float.
- Encoded 'tagText' into numerical format using Label Encoding.

### 3. Exploratory Data Analysis (EDA)
- Plotted the distribution of sales (sold) and prices.
- Created scatterplots showing relationships between price and sold units.
- Analyzed the impact of 'tagText' on sales distribution.
- Created pairplots for selected features.

### 4. Feature Engineering
- Calculated discount percentage if original price was available.
- Converted 'productTitle' to numerical vectors using TF-IDF (optional based on missing data).
- Encoded categorical features for machine learning.

### 5. Model Selection and Training
- Selected Linear Regression and Random Forest Regressor models.
- Performed train-test split (80 percent train, 20 percent test).
- Trained both models on training data.

### 6. Model Evaluation
- Evaluated both models using:
  - Mean Squared Error (MSE)
  - R-squared Score (R2)
- Printed model performance metrics.

### 7. Conclusion
- Random Forest model typically performed better due to its ability to capture non-linear relationships in complex datasets.
- Linear Regression performed adequately when assuming a linear relationship between features and target.
- Further tuning with hyperparameter optimization could improve performance.


