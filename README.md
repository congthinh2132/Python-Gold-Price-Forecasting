# 📈 Gold Price Forecasting

![Gold Price Forecasting](https://img.shields.io/badge/Status-Active-success)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This project utilizes advanced machine learning and deep learning techniques to forecast the daily closing price of gold. By analyzing historical data, the project implements and compares various time-series forecasting models to identify the most accurate predictor.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Models Implemented](#models-implemented)
- [Results & Evaluation](#results--evaluation)

## 🧐 Overview
The primary objective of this project is to predict the "Closing Price" of gold for the next trading day. The project explores a variety of statistical and neural network-based approaches to handle the volatility and non-linearity of financial time-series data.

## 🚀 Features
- **Data Acquisition**: Automated fetching of historical data from Yahoo Finance.
- **Preprocessing**: Cleaning, missing value handling, and normalization.
- **Exploratory Data Analysis (EDA)**: Visualization of trends, seasonality, and volatility.
- **Model Comparison**: Implementation of 6 different forecasting algorithms.
- **Evaluation**: Rigorous testing using RMSE, MSE, and MAE metrics.

## 📊 Dataset
The data is sourced from **Yahoo Finance** (Symbol: `GC=F`).
- **Source**: [Yahoo Finance Gold Futures](https://finance.yahoo.com/quote/GC=F/)
- **Interval**: Daily
- **Features Used**: Open, High, Low, Close, Volume.
- **Preprocessing**: A rolling window of **60 days** is used to create feature sequences for training the models.

## 📂 Project Structure
```bash
Python-Gold-Price-Forecasting/
├── data/                 # Raw and processed datasets
├── source_code/          # Jupyter notebooks and Python scripts
│   ├── ARIMA.ipynb
│   ├── LSTM.ipynb
│   ├── CNN_LSTM.ipynb
│   └── ... (other model scripts)
├── Paper.docx            # Research paper detailing the study
├── Report.docx           # Project report
└── README.md             # Project documentation
```

## 🧠 Models Implemented
The project evaluates the following models:

* **ARIMA (Autoregressive Integrated Moving Average):** For capturing linear trends in time series.
* **HMM (Hidden Markov Models):** To model hidden states in the market regime.
* **BNN (Bayesian Neural Networks):** Probabilistic modeling to capture uncertainty.
* **LSTM (Long Short-Term Memory):** Best for capturing long-term dependencies in sequence data.
* **GRU (Gated Recurrent Units):** A streamlined variation of LSTM.
* **CNN-LSTM:** A hybrid model using CNN to extract features and LSTM for sequence prediction.

## 📈 Results & Evaluation
Models are evaluated using the following metrics:

* **MSE** (Mean Squared Error)
* **RMSE** (Root Mean Squared Error)
* **MAE** (Mean Absolute Error)

> **Note:** Please refer to the `Report.docx` or the specific notebook outputs for the comparative analysis and to see which model yielded the best performance.

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
