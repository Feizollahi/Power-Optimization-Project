# Model 1 - Optimizing Revenue Generation

## How to run:

The user needs to input the desired date and time resolution (in minutes) to the main optimization algorithm. For example:

main_opt_algorithm(opt_date='2022-08-06',delta_t=5)
In this case, the model will optimize the revenue for 2022-08-06 with time resolution of 5 minutes. 

## Requirements:

- python 3.8.12
- numpy 1.20.3
- pandas 1.3.4
- matplotlib 3.5.0
- seaborn 0.11.2
- pyomo 6.5.0


## Model Description
The model reads the LBMP data for NYISO. Then, it optimizes the battery storage dispatch subject to the following constraint:

- Maximum discharge power capacity (kW)= 100 kW
- Maximum charge power capacity (kW)= 100 kW
- Discharge energy capacity (kWh)= 200 kWHr
- AC-AC Round-trip efficiency (%)=85%
- Maximum daily discharged energy limit (kWh)= 200KWHr



Details of the optimization model, decision variables, objective function and constraints are discussed in Model1-Optimization.ipynb.

## Model Outputs
The code outputs the following
- optimal total revenue
- total battery storage charging cost
- total battery storage discharged throughput
- an excel file including 
	o- LBMP,
	o- charge power, 
	o- discharge power,
	o-  net charge power,
	o-  storage energy level, and
	o-  revenue at each time stamp
- plot for the optimal schedule of charging and discharging along with the LBMP.


At the end of Model1-Optimization.ipynb, the results of the model for 2022-08-06 with time resolution of 5, 20 and 60 minutes are presented and discussed. Also some insights from the results and suggestions for improivement are provided.
