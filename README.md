# TCS Securities Lending & Borrowing (SLB) Market Analysis

## Project Overview
This is a finance-focused exploratory data analysis project using historical TCS Securities Lending & Borrowing (SLB) market data.

The project performs data cleaning, transformation, aggregation and visualization. No machine-learning model is used.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## Dataset
The dataset contains 230 SLB trading records across 110 trading dates and multiple settlement series.

Important fields include:
- Symbol
- Trading date
- Settlement date
- SLB series
- Open, high, low and close quote prices
- 52-week high and low
- Total traded quantity
- Total traded value
- Number of trades

## Data Cleaning
The project:
1. Removes extra spaces from column names.
2. Removes duplicate rows.
3. Parses trading and settlement dates.
4. Converts comma-formatted quantities, traded values and trade counts into numeric columns.
5. Converts price columns to numeric values.
6. Checks missing values after cleaning.

## Analysis Performed
- Summary statistics
- Most active SLB settlement series
- Daily total traded quantity
- Daily total traded value
- Daily number of trades
- Number of active series
- Weighted average SLB price
- Highest-volume trading days
- Highest-value trading days
- Correlation between market activity measures
- Distribution of weighted SLB prices

## Weighted Average Price
Because several SLB series may trade on the same day, the project calculates:

Weighted Average Price = Total Traded Value / Total Traded Quantity

This gives a simple daily measure of the average traded SLB price across active series.

