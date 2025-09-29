# Stock-Valuation-with-Dividend-Discount-Model-DDM-using-Python-AT-T-Case-Study
This project implements the Dividend Discount Model (DDM) in Python to value AT&amp;T (T) stock, inspired by the Coursera Guided Project 'Stock Valuation with Dividend Discount Model'. Instead of Excel, it uses web scraping for dividend data, yfinance for stock info, and calculations for growth rate, CAPM cost of equity, and fair value.

## Overview
The Dividend Discount Model (DDM) values a stock as the present value of expected future dividends.
- Scrapes historical dividends for AT&T investor site.
- Calculates annual dividends and median growth rate.
- Use CAPM for cost of equity (beta from yfinance, risk-free rate from 10Y Treasury Yield 4.19%, market return from S&P 500 (annual return (5Y CAGR) 14.68%) update on September 26 2025

      The latest date of the US10Y data: 2025-09-26
      10Y Treasury Yield (Risk-Free Rate): 4.19%
      Date range of S&P 500 data: 2020-09-28 to 2025-09-26
      S&P 500 Daily Return (5Y CAGR): 0.06%
      S&P 500 Annual Return (5Y CAGR): 14.68%

- Computes fair value: Next dividend/(Cost of Equity - Growth Rate)

## Key Features
- Web scraping with Selenium/BeautifulSoup
- Dividend aggregation and growth rate
- CAPM: Cost of equity = risk-free rate + beta + (market return - risk-free rate)

DDM formula: 

          Fair Value = D1 / (r - g)
          D1 = Dividend next year = D0 * (1 + g)
          r = Cost of Equity
          g = Growth rate of dividends (CAGR of dividends over the last 5 years)
          Where:
          - D0 = Most recent dividend
          - Cost of Equity = 0.12
          - Growth rate of dividends (g)

## Results
    Last Annual Dividend: $1.1100
    Next Year Dividend: $1.1396
    Fair Value of AT&T Stock: $12.2060
    Current Price of AT&T Stock: $28.3100
    Upside Potential of AT&T Stock: -56.88%
    The stock is overvalued.

## Visualizations

<img width="842" height="545" alt="Image" src="https://github.com/user-attachments/assets/570f547a-2f78-4e22-bda9-71bfacc2c604" />

## Contact
- Thanh Xuyen Nguyen
- LinkedIn: [xuyen-thanh-nguyen-0518](https://www.linkedin.com/in/xuyen-thanh-nguyen-0518/)
- Email: thanhxuyen.nguyen@outlook.com

Inspired by Coursera Project: https://www.coursera.org/projects/stock-valuation-dividend-discount-model
