📈 Stock Market Analysis and Visualization

Project Objective

This project implements a comprehensive stock market analysis tool in Python. It utilizes Pandas for data manipulation, NumPy for numerical calculations, and Matplotlib/Seaborn for visualizations. The goal is to analyze historical stock price data, calculate key technical indicators (like Moving Averages), and visualize trends, patterns, and correlations to support investment decisions.

Features

The core logic is encapsulated within the StockAnalyzer class and demonstrates the following functionalities:

Data Handling & NumPy Operations

Synthetic Data Generation: Generates a clean, synthetic dataset simulating historical stock prices, volume, and dates.

NumPy Integration: Converts critical Pandas Series (Close Price, Volume) to NumPy arrays.

Demonstrated Operations (NumPy): Indexing, Slicing, Element-wise Mathematical Operations (calculating Market Cap Index), and statistical Filtering (finding prices > 1 standard deviation).

Technical Analysis & Statistics

Indicator Calculation: Computes 20-Day and 50-Day Simple Moving Averages (SMA).

Daily Returns: Calculates daily percentage change in price.

Statistical Functions: Calculates Standard Deviation and 95th Percentile for Daily Returns, and aggregates Volume data (mean, max, min).

Visualization (Matplotlib & Seaborn)

The script generates two main figures:

Matplotlib Multi-Plot: A three-panel figure showing:

Line Plot: Closing Price vs. 20-Day and 50-Day SMAs (Identifying trends).

Bar Plot: Trading Volume over time.

Scatter Plot: Daily Return vs. Trading Volume (Analyzing volatility).

Seaborn Heatmap: A correlation matrix showing the linear relationship between key metrics (Close Price, SMAs, Volume, Daily Return).

Prerequisites

To run this project, you need the following Python libraries:

pip install pandas numpy matplotlib seaborn


How to Run the Script

Save the provided code as stock_analyzer.py.

Run the script from your terminal:

python stock_analyzer.py


Expected Output

Upon execution, the script will first print the results of the NumPy and Indicator calculations:

✅ Generated synthetic data for ticker: AAPL (252 trading days) starting from 2023-01-01.

StockAnalyzer initialized and core data converted to NumPy arrays.

--- NumPy Array Demonstration ---
1. Last closing price (Index -1): $146.55
...
4. Found 55 days with price > 1-Sigma.

--- Calculating Indicators ---
5. Daily Return Std Dev (std()): 1.1625
...
7. Aggregating Max/Min/Mean Volume:
mean    5581070
max     9944718
min     1075388
Name: Volume, dtype: int64

--- Generating Visualizations (Matplotlib & Seaborn) ---


Following the printed output, two separate visualization windows (or plots in the output display) will be generated: the three-panel Matplotlib figure and the Seaborn correlation heatmap.
