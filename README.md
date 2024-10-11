# Fractional Differentiation in Financial Data

## Project Overview

This project focuses on **fractional differentiation**, a technique described in *Advances in Financial Machine Learning* by Marcos Lopez de Prado. Fractional differentiation allows the transformation of time series data to make it stationary while retaining long-term memory, which is crucial for financial data analysis. The goal of this project is to implement fractional differentiation, validate the results using financial data, and compare the custom implementation with existing libraries like `mlfinlab` and `fracdiff`.

## Purpose

The primary objectives of this project are:
- **Self-education**: Understand the theory and application of fractional differentiation after reading *Advances in Financial Machine Learning*.
- **Practical Implementation**: Apply fractional differentiation to real-world stock market data and compare the custom implementation with established libraries.
- **Future Usage**: I plan to continue implementing techniques described by Marco Lopez de Prado and use them while analysing Financial data.
  
## Methodology

1. **Data Collection**: Yahoo data. Data from Apple (AAPL) historical stock prices were retrieved using the `yfinance` library.
2. **Custom Implementation**: A fractional differentiation function was developed in Python using the binomial expansion approach described in *Advances in Financial Machine Learning*.
3. **Comparison with Libraries**: Results from the custom implementation were validated by comparing with two libraries, `mlfinlab` and `fracdiff`.


## How to Run the Code

1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install yfinance fracdiff matplotlib
