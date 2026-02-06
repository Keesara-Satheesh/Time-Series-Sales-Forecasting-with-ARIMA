**Time Series Sales Forecasting with ARIMA**
**Project Overview**
This project focuses on forecasting monthly sales for the upcoming quarter using the ARIMA (AutoRegressive Integrated Moving Average) model. The analysis involves exploratory data analysis (EDA), stationarity testing, model parameter selection, and rigorous evaluation to ensure reliable business insights.

**Objectives**
Data Exploration: Analyze historical sales trends and seasonal patterns from 2013 to 2016.
Statistical Modeling: Implement an ARIMA model to capture the underlying temporal dependencies of the sales data.
Forecasting: Predict the next three months of sales with 95% confidence intervals.
Evaluation: Validate model performance using standard accuracy metrics (MAE and MAPE).

**Technologies Used**
Environment: Jupyter Notebook
Language: Python 3.x
Core Libraries:
pandas: Data manipulation and time-series alignment.
statsmodels: Statistical testing (ADF test) and ARIMA modeling.
matplotlib & seaborn: Visualization of trends, residuals, and forecasts.
scikit-learn: Error metric calculations.

**Methodology**
Data Preprocessing: Handled datetime parsing, set monthly frequency, and checked for missing values.
Stationarity Check: Conducted the Augmented Dickey-Fuller (ADF) test. Applied first-order differencing (
d=1) to transform the non-stationary series into a stationary one.
Model Selection: Utilized ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots to identify potential 
p and q parameters.
Validation: Performed a train-test split (using the final 6 months of 2016 as a test set) to calculate the Mean Absolute Percentage Error (MAPE).
Final Forecast: Refit the model on the entire dataset to generate the 3-month outlook.

**Deliverables**
sales_forecasting.ipynb: The complete Python notebook containing code, visualizations, and documentation.
monthly_sales.csv: The historical dataset used for training.
Visualizations:
Historical sales trend lines.
Stationarity and differencing plots.
3-Month forecast plot with shaded confidence intervals.

**How to Run**
Ensure you have Python installed with the required libraries:
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
Place the monthly_sales.csv in the same directory as the notebook.
Open sales_forecasting.ipynb in Jupyter Notebook or VS Code and run all cells.

**Results Summary**
The final model provides a quantitative basis for inventory and revenue planning. By accounting for historical growth and variance, the 3-month forecast assists stakeholders in making data-driven decisions for the next quarter.
