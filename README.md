# TCS Stock Price Forecasting

This project focuses on **forecasting the stock price of Tata Consultancy Services (TCS)**, a leading global IT services and consulting company, using advanced time series analysis and machine learning techniques. The goal is to predict future stock movements based on historical data, providing insights for potential investment strategies.

## Methodology

The forecasting process follows a rigorous data science pipeline, from data acquisition and exploratory analysis to model training and evaluation.

### 1. Data Acquisition and Preprocessing

*   **Data Source**: Historical stock data for TCS (ticker `TCS.NS`) is sourced from Yahoo Finance using the `yfinance` library, covering a period starting from January 1, 2010.
*   **Preprocessing**: The raw data undergoes cleaning steps, including handling multi-level column indexing, dropping redundant data, and verifying data integrity by checking for null or duplicate values.

### 2. Exploratory Data Analysis (EDA)

The EDA phase provides a deep understanding of the stock's historical behavior:

*   **Statistical Summary**: Descriptive statistics are generated to summarize the data distribution.
*   **Visualization**: Key visualizations include:
    *   **Correlation Heatmaps**: To understand the relationships between different stock features (Open, High, Low, Close, Volume).
    *   **Close Price History**: A time series plot of the closing price over the entire period.
    *   **Moving Averages**: Calculation and plotting of 100-day and 200-day moving averages to identify trends and potential support/resistance levels.

### 3. Forecasting Models

Two distinct and powerful models are employed to capture both trend-seasonality and complex sequential dependencies in the time series data:

| Model | Type | Purpose | Key Libraries |
| :--- | :--- | :--- | :--- |
| **Prophet** | Additive Regression Model | Excellent for capturing seasonality, holidays, and long-term trends in time series data. | `prophet` (from Meta) |
| **LSTM** | Deep Learning (Recurrent Neural Network) | Highly effective for modeling and predicting time series sequences by learning long-term dependencies. | `tensorflow`, `keras` |

## Project Structure

The repository is organized as follows:

| Directory/File | Description |
| :--- | :--- |
| `notebooks/` | Contains the main analysis file, `TCS_forecasting.ipynb`, which details the entire workflow from data loading to model prediction. |
| `presentation/` | Contains the project's final presentation in PDF format. |
| `README.md` | This file. |

## Technologies Used

The project is implemented entirely in Python and relies on the following key libraries:

*   `pandas`, `numpy`: Data manipulation and numerical operations.
*   `matplotlib`, `seaborn`, `plotly`: Data visualization and plotting.
*   `yfinance`: Historical stock data acquisition.
*   `prophet`: Time series forecasting.
*   `tensorflow`, `keras`: Deep learning framework for the LSTM model.

## Team

This project was developed by the following team members:

*   SeifElden Osama Hosney
*   Sama NigmEldin
*   Habiba Ashraf
*   Mohamed Badr
*   Esraa Ahmed
*   Mohamed AbdAlwanis
