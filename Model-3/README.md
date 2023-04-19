# Model 3 - NYISO Fuel Mix Data Analysis

 ## Model Description
 The model reads the fuel-mix generation data for the entire NYISO for year 2022. Then, it plots the generation and emission heat maps considering different times of day and dates of year. 

It also finds the average day which is obtained by the average across each timestamp for each day within the dataset. Then, the best match to the average date is considered as a typical day. The model analyzes the generation, emission and emission factor for average and typical days. 

It also presents the generation and emission by fuel category for the average day.

At the end of Model3-Fuelmix.ipynb, the some insights and suggestions are provided.


## How to run:

The user needs to input the desired start_date, end_date, and time resolution (in minutes) to the main fuel mix algorithm. For example:

main_fuelmix_alg(start_date='2022-01-01',end_date='2022-12-31',delta_t=5)

In this case, the model will analyze the generation and emission for the interval of start_date='2022-01-01' and end_date='2022-12-31' and time resolution delta_t=5.
	


 ## Requirements
 - python 3.8.12
- numpy 1.20.3
- pandas 1.3.4
- matplotlib 3.5.0
- seaborn 0.11.2


