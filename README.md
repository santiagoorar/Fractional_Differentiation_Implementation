# Fractional Differentiation in Financial Data

## Project Overview

This project focuses on **fractional differentiation**, a technique described in *Advances in Financial Machine Learning* by Marcos Lopez de Prado. Fractional differentiation allows the transformation of time series data to make it stationary while retaining long-term memory, which is crucial for financial data analysis. The goal of this project is to implement fractional differentiation, validate the results using financial data, and compare the custom implementation with existing libraries like `mlfinlab` and `fracdiff`.

## Purpose

The primary objectives of this project are:
- **Self-education**: Understand the theory and application of fractional differentiation after reading *Advances in Financial Machine Learning*.
- **Practical Implementation**: Apply fractional differentiation to real-world stock market data and compare the custom implementation with established libraries.
- **Future Usage**: I plan to continue implementing techniques described by Marco Lopez de Prado and use them while analysing Financial data.
  
## Mathematical Background

Fractional differentiation allows for partial differencing of a time series, retaining some of its long memory properties. The mathematical formula for fractional differentiation is derived from the binomial expansion:

\[
(1 - B)^d X_t = \sum_{k=0}^{\infty} \binom{d}{k} (-1)^k X_{t-k}
\]

Where:
- \( B \) is the backshift operator, such that \( B X_t = X_{t-1} \),
- \( d \) is the differentiation order, where \( 0 < d < 1 \),
- \( \binom{d}{k} \) are the binomial coefficients, defined as:

\[
\binom{d}{k} = \frac{d (d-1) (d-2) \cdots (d-k+1)}{k!}
\]

This method allows for more control over the differencing process, making it particularly useful in financial data where preserving memory is important.

## Methodology

1. **Data Collection**: Yahoo data. Data from Apple (AAPL) historical stock prices were retrieved using the `yfinance` library.
2. **Custom Implementation**: A fractional differentiation function was developed in Python using the binomial expansion approach described in *Advances in Financial Machine Learning*.
3. **Comparison with Libraries**: Results from the custom implementation were validated by comparing with two libraries, `mlfinlab` and `fracdiff`.


## How to Run the Code

1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install yfinance fracdiff matplotlib
