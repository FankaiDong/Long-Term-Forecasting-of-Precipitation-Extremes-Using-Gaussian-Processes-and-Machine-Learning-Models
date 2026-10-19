# Long-Term-Forecasting-of-Precipitation-Extremes-Using-Gaussian-Processes-and-Machine-Learning-Models

## 1. Project Overview
This repository contains the Python code and dataset used for an MSc dissertation at The University of Manchester.
This study aims to compare four machine learning models for predicting extreme precipitation events in London: Gaussian Process (GP), XGBoost, LightGBM and Long Short-Term Memory (LSTM).
A two-stage forecasting framework is adopted. The first stage uses classification models to predict the probability of extreme precipitation occurrence, while the second stage uses regression models to predict precipitation intensity on extreme days. The models are evaluated using classification and regression metrics. Based on the results, a final two-stage model is selected and further evaluated at different forecasting horizons.

## 2. Dataset
This study uses extreme precipitation indicator data for London obtained from the Copernicus Climate Data Store (CDS).
The dataset, `london_precip_extreme_index_95th_1989_2018.csv`, contains daily precipitation indicators from 1989 to 2018. Several predictive features are constructed from the data, including lagged variables, rolling statistics, historical extreme event indicators and seasonal features.
**Data source:** https://cds.climate.copernicus.eu/datasets/sis-european-risk-extreme-precipitation-indicators?tab=overview

## 3. Repository Contents
This repository contains two main files:

**1. `ERP_final.ipynb`**
This Jupyter Notebook contains all Python code used in the study, including:
- Data preprocessing and feature engineering
- Exploratory Data Analysis
- Gaussian Process classification and regression
- XGBoost classification and regression
- LightGBM classification and regression
- LSTM classification and regression
- Feature selection and model evaluation
- Development and evaluation of the final two-stage model
- Rolling forecasting at 1-day, 3-day and 7-day horizons

**2. `london_precip_extreme_index_95th_1989_2018.csv`**
This file contains the daily extreme precipitation indicators for London from 1989 to 2018. It is used for model training, testing and forecasting analysis.

## 4. Requirements
The experiments were developed in Python, mainly using Google Colab.
The main Python libraries used in this study include:
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- XGBoost
- LightGBM
- TensorFlow / Keras
- Statsmodels

## 5. How to Run
1. Download `ERP_final.ipynb` and `london_precip_extreme_index_95th_1989_2018.csv` from this repository.
2. Open `ERP_final.ipynb` in Google Colab or another compatible Jupyter Notebook environment.
3. Install any missing Python libraries if required.
4. Upload the CSV file to the working environment and check the data file paths in the notebook to ensure that the dataset can be loaded correctly.
5. Run the notebook cells in sequence to reproduce the data processing, model training, evaluation and forecasting experiments.

## 6. Additional Notes
The `ERP_final.ipynb` file contains the whole experimental code used in this dissertation.
The main research methodology, experimental results and discussion are presented in the dissertation report.
