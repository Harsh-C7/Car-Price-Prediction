# Car Price Prediction

This project demonstrates a machine learning approach to predict the selling price of cars using the Lasso regression model. The dataset used in this project is a car dataset that includes various features of cars and their corresponding selling prices.

## Overview

The code performs the following steps:

1. **Import Libraries**: Essential libraries such as [Pandas](https://pandas.pydata.org/) for data manipulation, [Matplotlib](https://matplotlib.org/) and [Seaborn](https://seaborn.pydata.org/) for data visualization, and [Scikit-learn](https://scikit-learn.org/stable/) for model training and evaluation are imported.

2. **Data Loading and Exploration**:
   - The dataset is loaded using Pandas.
   - Initial exploration is done using `head()` to view the first few rows of the dataset.
   - The distribution of the `Fuel_Type` feature is examined using `value_counts()`.

3. **Data Preprocessing**:
   - The `Fuel_Type` categorical variable is encoded into numerical values: Petrol as 0, Diesel as 1, and CNG as 2.
   - The features `Car_Name` and `Selling_Price` are separated, with `Car_Name` being dropped from the features set `x` and `Selling_Price` being used as the target variable `y`.

4. **Data Splitting**:
   - The dataset is split into training and testing sets using a 90-10 split.

5. **Model Training**:
   - A Lasso regression model is initialized and trained on the training data.
   - The model's performance is evaluated using the R-squared metric on both the training and testing datasets.

6. **Visualization**:
   - Scatter plots are created to visualize the relationship between actual and predicted selling prices for both the training and testing datasets. The plots help in assessing the model's prediction accuracy visually.

## Results

- The model achieves an R-squared score of approximately 0.84 on both the training and testing datasets, indicating a good fit to the data.

## Usage

To use this code, ensure you have the necessary libraries installed and the dataset available at the specified path. You can modify the dataset or model parameters to explore different scenarios and improve prediction accuracy.
