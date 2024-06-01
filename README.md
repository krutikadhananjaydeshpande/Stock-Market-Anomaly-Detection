# Stock Market Anomaly Detection

This repository contains a Python script for detecting anomalies in stock market data using statistical methods. The script analyzes historical price and volume data for a set of stocks and identifies unusual patterns or behaviors that deviate significantly from the expected norm.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Anomaly detection in the stock market is crucial for identifying potential opportunities or risks. By detecting unusual price movements or trading volumes, investors can gain insights into market trends, company-specific events, or broader market shifts. This script provides a framework for detecting and analyzing anomalies in stock market data using Python and various data analysis libraries.

## Requirements

To run the script, you need the following dependencies:

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- yfinance
- scipy

## Installation

1. Clone the repository:

git clone https://github.com/your-username/Stock-Market-Anomaly-Detection.git

2. Install the required dependencies:

pip install -r requirements.txt

## Usage

1. Open the Jupyter Notebook file `stock_market_anomaly_detection.ipynb`.

2. Run the notebook cells sequentially to execute the script.

3. The script will collect historical stock market data for a set of predefined tickers using the yfinance API.

4. It will preprocess the data, perform exploratory data analysis, and detect anomalies using the Z-score method.

5. The script will generate visualizations of the adjusted close prices, trading volumes, and detected anomalies for each stock.

6. It will also analyze the correlations between anomalies across different stocks and assign risk ratings based on the frequency and magnitude of anomalies.

7. The results and insights will be displayed in the notebook.

## Data

The script uses historical stock market data collected from the yfinance API. The data includes the following information for each stock:

- Date
- Open price
- High price
- Low price
- Close price
- Adjusted close price
- Trading volume

The script currently analyzes data for a one-year period from June 2022 to June 2023 for the following stocks:

- Apple Inc. (AAPL)
- Alphabet Inc. (GOOG)
- Microsoft Corporation (MSFT)
- Netflix, Inc. (NFLX)
- Tesla, Inc. (TSLA)

## Methodology

The script employs the following methodology for stock market anomaly detection:

1. Data Collection: Historical stock market data is collected using the yfinance API for a specified time period.

2. Data Preprocessing: The collected data is preprocessed to create a clean and structured dataset suitable for analysis.

3. Exploratory Data Analysis: The script generates visualizations of the adjusted close prices and trading volumes over time for each stock to identify trends and patterns.

4. Anomaly Detection: The Z-score method is used to identify anomalies based on how many standard deviations a data point is from the mean. A threshold of Z-score greater than 2 or less than -2 is used to flag anomalies.

5. Correlation Analysis: The script examines the correlations between anomalies across different stocks to identify potential market-wide events or sector-specific factors influencing the anomalies.

6. Risk Analysis: A risk rating is assigned to each stock based on the frequency and magnitude of anomalies detected in both price and volume data.

## Results

The script generates visualizations and insights into the stock market anomalies, including:

- Graphs of adjusted close prices and trading volumes over time for each stock
- Plots highlighting anomalies in adjusted close prices and trading volumes
- Correlation matrix showing the relationships between anomalies across different stocks
- Risk ratings assigned to each stock based on the frequency and magnitude of anomalies

The results provide valuable information for investors to make more informed decisions regarding potential opportunities or risks in the market.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

