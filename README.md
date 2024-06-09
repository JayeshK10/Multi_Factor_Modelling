# Project Overview

This project involves creating a multi-factor model using preprocessed real data from 2004 to 2010. The objective is to predict stock returns and use these predictions to compute the Markowitz portfolio. The project is divided into three main tasks:

1. **Developing a Factor Model**: Selecting multiple alpha factors and creating a composite alpha factor using various regression models.
2. **Computing the Markowitz Portfolio**: Using the derived factors to compute the Markowitz portfolio for each date in the sample.
3. **Qualitative Analysis**: Conducting qualitative analysis through various plots.

## Data Description

- **Data Period**: 2004-2010
- **Train/Validation Period**: 2003-2007
- **Test Period**: 2008-2010

### Data Structure

The data is stored in a dictionary where keys are dates, and the values are dataframes containing daily cross-sectional data. Each row in the dataframe corresponds to a particular stock, with multiple columns representing various attributes of the stock.

### Target Variable

- **Return ("Ret")**: The variable we aim to predict.

## Task 1: Developing a Factor Model

### Steps

1. **Factor Selection**: Identified multiple alpha factors relevant to predicting stock returns.
2. **Model Implementation**:
    - **Lasso Regression**
    - **Ridge Regression**
    - **Polynomial Functions**
    - **Ordinary Least Squares (OLS) Estimators**
3. **Composite Factor Creation**: Combined the selected alpha factors to create a composite alpha factor.
4. **Model Evaluation**: Calculated mean factor returns for the composite factor.

### Output

- Mean factor returns for the composite factor, which serves as an indicator of the factor model's predictive power.

## Task 2: Computing the Markowitz Portfolio

### Steps

1. **Factor Utilization**: Used the composite alpha factor derived from Task 1.
2. **Portfolio Construction**: Applied the Markowitz portfolio optimization method to construct portfolios for each date in the sample.
3. **Optimization**: Focused on maximizing return for a given level of risk.

### Output

- Optimized portfolios for each date, based on the Markowitz model.

## Task 3: Qualitative Analysis

### Steps

1. **Data Visualization**: Created various plots to analyze the data qualitatively.
2. **Analysis**: Interpreted the visualizations to gain insights into the data and the effectiveness of the models.

### Plots

- Time series plots of factor returns.
- Scatter plots of predicted vs. actual returns.
- Risk-return plots for the Markowitz portfolios.
- Histograms of stock returns and factor values.

## Conclusion

This project successfully implemented a multi-factor model to predict stock returns and used these predictions to construct optimized portfolios. The qualitative analysis provided additional insights into the data and the models' performance.

## Files and Directories

- **scripts/**: Contains the scripts for data processing, model implementation, and visualization.
- **results/**: Contains the output results, including model evaluations and plots.
- **README.md**: This readme file.

## How to Run the Project

1. **Colab Code**: Ensure the data files path is correctly updated. Run the rest code as it is. 

## Dependencies

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- statsmodels
- patsy
- statistics
