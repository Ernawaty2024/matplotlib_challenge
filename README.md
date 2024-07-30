# Evaluating the Efficacy of Capomulin: A Comprehensive Analysis of Pymaceuticals' Drug Performance

## Overview
This project utilized Matplotlib, Pandas, Scipy, and Sklearn to analyze and report the performances of Pymaceuticals' drug, Capomulin, against the other treatments regimes, highlighting key metrics such as tumor size reducation. The data was gathered from the most recent animal study involving 249 mice with SCC tumors. Observation and measurement of the tumor development were conducted over the course of 45 days. The analysis includes summaries and data visualizations using tables and charts.

### Key Componenets of the Report
1. **Data Preparation**
   - Opened Jupyter Notebook file <code style ="color:blue">[Pymaceuticals.ipynb](https://github.com/Ernawaty2024/matplotlib_challenge/blob/main/Pymaceuticals/Pymaceuticals.ipynb)</code>
   - The <code style ="color:blue">[Mouse_metadata](https://github.com/Ernawaty2024/matplotlib_challenge/blob/main/data/Mouse_metadata.csv)</code> and <code style ="color:blue">[Study_results](https://github.com/Ernawaty2024/matplotlib_challenge/blob/main/data/Study_results.csv)</code> DataFrames were merged into a single DataFrame.
   - A cleaned DataFrame was done on the unique mice IDs by removing any mouse ID with duplicated time points.
   
2. **Statistics Summary**
   - A DataFrame was created to include an indexed column of each drug regimen.
   - Calculation based on tumor volume: mean, median, variance, standard deviation, and SEM.
   
3. **Data Visualization**
    - Bar Charts
       - To show the total number of rows(Mouse ID/Timepoints) for each drug regimen throughout the study with Pandas `DataFrame.plot()` and Matplotlib `pyplot` methods
       
    - Pie Charts
        - To show the distribution of female versus male mice using Pandas `DataFrame.plot()` and Matplotlib `pyplot` methods
       
    - Box Plot
       - To show the distribution of the final tumor volume for all the mice in each treatment group and any potential outliers are hightlighted.
       - The quartiles and IQR were calculated after final tumor volume of each mouse was gathered across four most promising treatment regimes: Capomulin, Ramicane, Infubinol, and Ceftamin.
       - Determined any potential outliers by using the upper and lower bounds.
       
    - Line Plot
       - To show the line visualization of tumor volume versus time point for a single mouse that was treated with Capomulin.

    - Scatter Plot
       - To show the distribution of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

    - Linear Regression Model
       - To show the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatement regimen.


