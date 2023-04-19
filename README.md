# Power Project: Optimization, Forecasting and Fuel Mix Analysis for NYISO

This project includes 3 models:

## Model 1 - Optimizing Revenue Generation
In Model-1 directory, you can find the Model1-Optimization.ipynb Jupyter Notebook file and the coresponding README.md for descriptions.
The model reads the LBMP data for NYISO. Then, it optimizes the battery storage dispatch.


## Model 2 - Forecasting Electricity Prices
In Model-2 directory, you can find the Model2-Forecasting.ipynb Jupyter Notebook file and the coresponding README.md for descriptions.
This model uses LSTM to predict hourly LBMP for a given date based on the historical LBMPs.

## Model 3 - NYISO Fuel Mix Data Analysis
In Model-3 directory, you can find the Model3-Fuelmix.ipynb Jupyter Notebook file and the coresponding README.md for descriptions.
The model reads the fuel-mix generation data for the entire NYISO for year 2022. Then, it plots the generation and emission heat maps considering different times of day and dates of year. 

## Requirements
- python 3.8.12
- numpy 1.20.3
- pandas 1.3.4
- matplotlib 3.5.0
- seaborn 0.11.2
- pyomo 6.5.0
- torch 1.10.1

## GitHub url

https://github.com/Feizollahi/Power-Project.git

