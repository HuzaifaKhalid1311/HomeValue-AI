# HomeValue AI: Real Estate Price Predictor

## Overview
HomeValue AI is a machine learning project designed to estimate real estate market values based on property features. This repository contains the Phase 1 implementation, focusing on data preprocessing, exploratory data analysis (EDA), and baseline regression modeling.

## Features
* **Exploratory Data Analysis:** Visualizations of housing distributions, categorical trends, and price correlations.
* **Data Preprocessing:** Handling missing values, outlier mitigation, and data type conversions.
* **Predictive Modeling:** Implementation of regression algorithms to estimate continuous price variables.

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn
* **Environment:** Jupyter Notebook

## Project Structure
* `/data/` - Contains the raw housing dataset (e.g., CSV files).
* `/notebooks/` - Jupyter notebooks containing the EDA and model training code (`Part1_Submission.ipynb`).
* `README.md` - Project documentation.
* `requirements.txt` - Required Python dependencies.

## Models Implemented
1. **Multiple Linear Regression:** Serves as the interpretable baseline model to establish fundamental linear weights between property features (like Area and Bedrooms) and Price.
2. **Random Forest Regressor:** An advanced, ensemble-based model utilized to handle non-linear relationships and improve prediction accuracy across diverse neighborhoods.
