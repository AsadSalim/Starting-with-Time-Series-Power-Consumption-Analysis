# Starting-with-Time-Series-Power-Consumption-Analysis

# Project Overview
- My first project with Time Series using the Hourly Energy Consumption Dataset
- Data has been cleaned and analyzed
- Time Series Cross Validation has been utilized to train the model
- The XGBoost model has been used to predict the future

# Code and Resources
- Inspired by the following tutorials:
https://www.youtube.com/watch?v=vV12dGe_Fho&t=23s
https://www.youtube.com/watch?v=z3ZnOW-S550&t=596s
- link to the data: https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption?select=PJME_hourly.csv
- Python Version: 3.9
- Packages: pandas, numpy, sklearn, matplotlib, seaborn, xgboost

# Data Cleaning
Not so much cleaning was needed. The time column need to be reformatted as a datetime, then put it as an index to
the dataset. 
After that we analyzed the dataset visually (which was really powerful and intuitive technique) and removed the outliers found.

# Analysis
- The dataset has been analyzed visually using different visuals.
- New features has been added for more detailed analysis
- Lag features has been added, which turned out to be really important for the model later.

# Model Building
- Time Series cross-validator has been used which provides train/test indices to split time 
series data samples that are observed at fixed and higher time intervals than before, and thus shuffling is inappropriate.
- XGBRegressor has been utilized as the main model for the project.
