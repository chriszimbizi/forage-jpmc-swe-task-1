# Task 1: Interface with a Stock Price Data Feed

## Overview

In this task, modifications were made to `client3.py` to correct inaccuracies in stock price and ratio calculations. The changes address the following issues:

- Issue 1: Ratio output in the client was always 1.
- Issue 2: Stock prices were identical to bid prices.

## Changes Made

### `getDataPoint` method

- Updated to compute the average price using `(bid_price + ask_price) / 2` for accurate stock pricing.

### `getRatio()`

- Corrected to return the ratio of `price_a` to `price_b` and handle division by zero.

### `client3.py`

- Implemented a dictionary to store stock prices and used it to correctly calculate and print the stock ratio.

### Testing

- Verified correct stock prices and ratio calculations.
- Ensured output reflects accurate stock data.
