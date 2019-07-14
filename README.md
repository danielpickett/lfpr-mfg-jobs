# LFPR and Manufacturing Jobs

A Jupyter Notebooks project comparing time series data for labor force participation rates and manufacturing jobs.

This notebook was inspired by claims made by a 2020 Democratic presidential candidate regarding the impact of manufacturing job loss on the overall labor force participation rate. More specifically, there was a claim that men in particular are dropping out of the labor force due to the impact of automation on manufacturing jobs.

My goal was to compare changes in the labor force participation rate (LFPR) to changes in the number of employees working in manufacturing. If manufacturing job loss is impacting the LFPR, or it is impacting the LFPR for men dramatically more than it is for women, then I had hoped to see it in the data visualizations.

### TERMS:
Labor Force Participation Rate (LFPR): This includes all individuals who have a job and those who are looking for a job. This is important because the unemployment rate does not include people who are not working and are not looking for work. For example, the unemployment rate may be under 4%, but there may be more than a third of the population not participating in the labor force. Individual's are only counted as "unemployed" if they are looking for work, but there may be another portion of the population that has become so discouraged about their job outlook that they stopped looking and are therefore no longer counted as "unemployed".


### DATA:

The time series data I used in this project was sourced from FRED (https://fred.stlouisfed.org).

Here is a list of the datasets used.

Civilian Labor Force Participation Rate https://fred.stlouisfed.org/series/LNU01300000

Civilian Labor Force Participation Rate: Men https://fred.stlouisfed.org/series/LNS11300001

Civilian Labor Force Participation Rate: Women https://fred.stlouisfed.org/series/LNU01300002

All Employees: Total Nonfarm Payrolls https://fred.stlouisfed.org/series/PAYEMS

All Employees: Manufacturing https://fred.stlouisfed.org/series/MANEMP

### Analysis
To achieve this comparison, I pulled in the LFPR data for all workers, for men, and for women. This helped me see whether any specific changes to overall LFPR affected men more than women. Then I pulled in the time series showing all employees (nonfarm was as close as I could get to 'all') and compared that to the time series for all workers in manufacturing. To compare LFPR to manufacturing jobs, I converted manufacturing jobs to a percentage of all nonfarm jobs. Then I was able to add four total lines to my plot: LFPR, LFPR for men, LFPR for women, and manufacturing jobs as a percent of all nonfarm jobs.


### Steps to Run
1. Run `Jupyter Notebook` in repo directory
2. Open `LFPR and Manufacturing Jobs.ipynb`

Note: You can also preview the `.ipynb` file directly in GitHub

### Dependencies
1. sqlite3
2. pandas
3. datetime
