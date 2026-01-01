# TCS Stock Price Forecasting

## 1. Project Overview

This repository contains a comprehensive data science project focused on predicting the future stock prices of **Tata Consultancy Services (TCS)**, a leading global IT services and consulting company. The primary goal is to leverage historical stock market data and advanced machine learning techniques to build and evaluate predictive models.

The project follows a standard data science workflow, including data acquisition, exploratory data analysis (EDA), rigorous preprocessing, and the implementation of both traditional and deep learning models. The final analysis provides a comparative study of model performance to identify the most effective approach for time series forecasting in this context.

## 2. Methodology

### 2.1. Data Acquisition
Historical stock data for TCS (ticker: `TCS.NS`) was sourced from Yahoo Finance using the `yfinance` library. The dataset spans from January 1, 2010, to the present, providing a robust time series for training and testing the models.

### 2.2. Exploratory Data Analysis (EDA)
The initial analysis involved:
*   **Statistical Summary:** Generating descriptive statistics of the stock features (Open, High, Low, Close, Volume).
*   **Data Quality Check:** Verifying for missing values and duplicates.
*   **Correlation Analysis:** Visualizing the correlation between different features using a heatmap.
*   **Trend Analysis:** Plotting the historical closing price and analyzing long-term trends using 100-day and 200-day moving averages.

### 2.3. Data Preprocessing
The data was prepared for modeling through the following steps:
1.  **Feature Selection:** The 'Close' price was selected as the target variable for forecasting.
2.  **Scaling:** All features were scaled using `MinMaxScaler` to normalize the data between 0 and 1, which is crucial for deep learning models like LSTM.
3.  **Time-Step Creation:** For the LSTM model, the data was restructured into sequences (time steps) to capture temporal dependencies.

### 2.4. Models Implemented
Three distinct models were implemented and compared:

| Model | Type | Library | Key Characteristics |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | Traditional ML | Scikit-learn | Simple, fast, and provides a baseline for performance. |
| **Random Forest Regressor** | Ensemble ML | Scikit-learn | Non-linear model, robust to outliers, and less prone to overfitting. |
| **Long Short-Term Memory (LSTM)** | Deep Learning | TensorFlow/Keras | Recurrent Neural Network (RNN) variant, highly effective for sequential data like time series. |

## 3. Results and Model Comparison

The models were evaluated using standard regression metrics: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R2 Score.

The **Linear Regression** model showed a high R2 score on the training data, indicating a strong fit to the historical trend. However, the **LSTM** model demonstrated superior performance in capturing the complex, non-linear patterns of the stock price, resulting in a lower RMSE on the test set, which is a more reliable measure of forecasting accuracy.

The project includes a detailed visualization comparing the actual stock price against the predictions from the Linear Regression and Random Forest models, as well as a separate plot for the LSTM predictions. A final bar chart provides a clear comparison of the MAE and RMSE across all three models.

## 4. Repository Structure

```
TCS_forecasting/
├── notebooks/
│   └── TCS_forecasting.ipynb  # Main Jupyter Notebook with all code and analysis
├── presentation/
│   └── (Presentation files)     # Project presentation materials
└── README.md                  # This file
```

## 5. Installation and Usage

To replicate this analysis, follow these steps:

### Prerequisites
Ensure you have Python 3.x installed.

### Setup
1.  Clone the repository:
    ```bash
    git clone https://github.com/SeifEldenOsama/TCS_forecasting.git
    cd TCS_forecasting
    ```
2.  Install the required libraries. The main dependencies include `pandas`, `numpy`, `scikit-learn`, `tensorflow`, and `yfinance`.
    ```bash
    pip install pandas numpy scikit-learn tensorflow yfinance matplotlib seaborn
    ```

### Running the Analysis
1.  Open the Jupyter Notebook:
    ```bash
    jupyter notebook notebooks/TCS_forecasting.ipynb
    ```
2.  Run all cells in the notebook sequentially to execute the data acquisition, preprocessing, model training, and evaluation steps.

## 6. Team

This project was developed by the following team members:
*   SeifElden Osama Hosney
*   Sama NigmEldin
*   Habiba Ashraf
*   Mohamed Badr
*   Esraa Ahmed
*   Mohamed AbdAlwanis
