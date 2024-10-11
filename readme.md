
# Share Market Price Prediction

## Project Overview
This project aims to predict the closing prices of a company's stock based on historical market data using machine learning techniques. The prediction model uses a **Linear Regression** algorithm to forecast future prices based on features such as Open, High, Low, and Close prices from historical records.

## Data Source
The data for this project comes from the CSV file containing historical stock prices for a company, including the following columns:
- **Date**: The date of the stock data entry
- **Open**: The opening price of the stock
- **High**: The highest price of the stock during the trading day
- **Low**: The lowest price of the stock during the trading day
- **Close**: The closing price of the stock
- **Adj Close**: The adjusted closing price (corrected for splits and dividends)
- **Volume**: The number of shares traded

## Dependencies
The project requires the following libraries:
- **Pandas**: For data manipulation and analysis
- **NumPy**: For numerical computations
- **Scikit-learn**: For machine learning model implementation
    - `train_test_split`: For splitting the data into training and testing sets
    - `LinearRegression`: For applying linear regression to the data
    - `mean_squared_error`, `mean_absolute_error`: For evaluating model performance
- **Matplotlib**: For basic data visualization
- **Plotly**: For advanced, interactive visualizations

## Installation
To install the required libraries, run the following command:
```bash
pip install pandas numpy scikit-learn matplotlib plotly
```

## Steps
1. **Load the Data**: The dataset is loaded from a CSV file (`3MINDIA.BO.csv`), which contains historical stock data.
2. **Data Exploration**: 
    - Basic information about the dataset is printed using `data.info()`.
    - Descriptive statistics are generated using `data.describe()`.
3. **Data Preprocessing**: 
    - Data is split into training and testing sets using the `train_test_split` function from Scikit-learn.
4. **Model Training**:
    - A linear regression model is trained on the data.
    - The model predicts the stock's closing prices based on historical data.
5. **Model Evaluation**: 
    - The model's performance is evaluated using mean squared error and mean absolute error metrics.
6. **Visualization**: 
    - Matplotlib and Plotly are used to create visualizations of the stock price trends and the model's predictions.

## Usage
To run the project, ensure that you have the required dependencies installed and execute the Jupyter Notebook.
