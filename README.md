# EDA and ARIMA/SARIMA Modeling on GE Last 3-Year Adj Close Stock Price

This repository provides a detailed guide for performing Exploratory Data Analysis (EDA) on the General Electric (GE) stock price data for the last 3 years. It also includes the process of building ARIMA and SARIMA models to forecast the stock price.

## Notebook
The notebook `eda_and_arima_sarima_ge_stock.ipynb` contains the complete code, step-by-step explanations, and visualizations for the EDA and modeling tasks. It is recommended to open and run the notebook in a Jupyter Notebook environment to follow along with the analysis.

## Dataset
The dataset used in this analysis is the adjusted closing stock price of General Electric (GE) for the past 3 years. The data is assumed to be available in a CSV file named `ge_stock_price.csv`. The dataset should contain two columns:

- Date: The date of the stock price in a YYYY-MM-DD format.
- Adj Close: The adjusted closing price of GE stock.

Ensure that the dataset is in the correct format and located in the same directory as the notebook or update the notebook code accordingly to load the data from the appropriate file path.

## Setup and Dependencies
To run the notebook successfully, you need to have the following dependencies installed:

- Python (version 3.6 or above)
- Pandas: A powerful data manipulation library
- NumPy: A fundamental package for scientific computing with Python
- Matplotlib: A plotting library for creating visualizations
- Statsmodels: A library for time series analysis and modeling

You can install the required Python packages by running the following command in your terminal or command prompt:
```
pip install pandas numpy matplotlib statsmodels
```

## EDA (Exploratory Data Analysis)
The EDA process helps us understand the GE stock price data and uncover any patterns, trends, or anomalies. The notebook covers the following EDA tasks:

1. Data loading: The dataset is loaded using the Pandas library, and the necessary columns are extracted for analysis.
2. Data cleaning: The data is checked for missing values, outliers, and inconsistencies. If required, data cleaning techniques such as interpolation or removal of outliers can be applied.
3. Descriptive statistics: Summary statistics such as mean, median, standard deviation, and percentiles are calculated to understand the central tendencies and spread of the data.
4. Data visualization: Various plots, including line plots, histograms, and scatter plots, are created to visualize the stock price over time, explore the distribution of prices, and identify any seasonality or trends.
5. Time series decomposition: The time series is decomposed into its components, including trend, seasonality, and residual, using methods like moving averages or the STL decomposition.
6. Autocorrelation analysis: Autocorrelation and partial autocorrelation plots are generated to examine the correlation between the stock price and its lagged values, helping to identify potential AR and MA components for the ARIMA or SARIMA models.
7. Stationarity check: The stationarity of the time series is assessed using statistical tests like the Augmented Dickey-Fuller (ADF) test to determine if differencing is required.

## ARIMA and SARIMA Modeling
The notebook walks you through the steps of building ARIMA and SARIMA models to forecast the GE stock price. The ARIMA models are suitable for non-seasonal data, while SARIMA models are appropriate for data exhibiting seasonality. The modeling tasks include:

1. Model order selection: The optimal order (p, d, q) for the ARIMA model and the seasonal order (P, D, Q, m) for the SARIMA model are determined using criteria such as AIC,

 BIC, or cross-validation.
2. Model fitting: The selected ARIMA or SARIMA model is fitted to the historical data to estimate the model parameters.
3. Diagnostic checking: The residuals of the model are analyzed for stationarity, autocorrelation, and normality. Diagnostic plots such as ACF and PACF plots, QQ plots, and residual histograms are created to assess the model's goodness of fit.
4. Forecasting: Using the fitted ARIMA or SARIMA model, future predictions of the GE stock price are generated. The forecasts are visualized alongside the historical data to evaluate the model's performance.

## Usage
To use this repository, follow these steps:

1. Clone or download the repository to your local machine.
2. Install the necessary dependencies by running `pip install pandas numpy matplotlib statsmodels` in your terminal or command prompt.
3. Open the `GE_Stock_Predriction_And_Forecasting.ipynb` notebook in a Jupyter Notebook environment.
4. Execute the cells in the notebook sequentially to perform EDA, build the ARIMA and SARIMA models, and generate forecasts.

It is recommended to go through the code, understand the explanations, and adapt the analysis as per your specific requirements. Feel free to modify the notebook and experiment with different settings, techniques, or models.

Please note that stock price forecasting is a challenging task, and the accuracy of the models heavily depends on various factors, including the nature of the data, market conditions, and external events. Use the models with caution and always validate the results with additional analysis or domain expertise.

If you have any questions or need further assistance, please don't hesitate to reach out.
