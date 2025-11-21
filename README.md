# Task-4-stock-intraday-calculation-
This Python script helps you backtest intraday trading strategies using 1-minute interval data from Yahoo Finance (via yfinance). It calculates daily P&amp;L (profit &amp; loss) based on fixed entry and exit times for any stock index or equity.

Features

✔ Fetches 1-minute OHLC data automatically using yfinance
✔ Allows you to set entry time, exit time, and date range
✔ Automatically filters the nearest candle for entry and exit
✔ Calculates daily P&L and total P&L
✔ Outputs a clean pandas DataFrame summary

How It Works

The script downloads 1-minute stock data (OHLCV) for the selected period.
Extracts date and time from the timestamp.
For each trading day:
Finds the first candle at or after entry time
Finds the last candle at or before exit time
Calculates P&L = Exit Price − Entry Price
Shows:
Daily Entry/Exit prices
Daily P&L
Total P&L for the entire period
