# 📈 TCS Stock Price Forecasting 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)](https://www.tensorflow.org/)

A comprehensive data science project focused on predicting the future stock prices of **Tata Consultancy Services (TCS)** using historical market data and advanced machine learning techniques.

## 🌟 Project Overview

This repository leverages a standard data science workflow to build and evaluate predictive models for stock market forecasting. The project compares traditional machine learning models with deep learning architectures to identify the most effective approach for time series analysis.

### Key Objectives:
- **Data Acquisition**: Automated retrieval of historical stock data using `yfinance`.
- **Exploratory Data Analysis (EDA)**: In-depth trend analysis, statistical summaries, and correlation studies.
- **Predictive Modeling**: Implementation of Linear Regression, Random Forest, and Long Short-Term Memory (LSTM) networks.
- **Performance Evaluation**: Comparative analysis using MAE, RMSE, and R² metrics.

## 📂 Repository Structure

```text
.
├── notebooks/              # Core analysis and modeling
│   └── TCS_forecasting.ipynb # Main Jupyter Notebook
├── presentation/           # Project presentation materials
│   └── TCS_presentation.pdf
├── requirements.txt        # Project dependencies
├── LICENSE                 # MIT License
└── README.md               # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or Google Colab

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/SeifEldenOsama/TCS_forecasting.git
   cd TCS_forecasting
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/TCS_forecasting.ipynb
   ```
2. Run the cells sequentially to reproduce the analysis and model training.

## 📊 Model Comparison

| Model | Type | Library | Performance Note |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | Traditional ML | Scikit-learn | Baseline performance for linear trends. |
| **Random Forest** | Ensemble ML | Scikit-learn | Robust to outliers and non-linear patterns. |
| **LSTM** | Deep Learning | TensorFlow | Superior at capturing complex temporal dependencies. |

## 🤝 Team

Developed by:
- **SeifElden Osama Hosney**
- **Sama NigmEldin**
- **Habiba Ashraf**
- **Mohamed Badr**
- **Esraa Ahmed**
- **Mohamed AbdAlwanis**

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Developed with ❤️ for Financial Analytics
