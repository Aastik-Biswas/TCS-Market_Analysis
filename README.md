# TCS Securities Lending & Borrowing (SLB) Market Analysis

## Project Overview
This is a finance-focused exploratory data analysis project using historical TCS Securities Lending & Borrowing (SLB) market data.

The project performs data cleaning, transformation, aggregation and visualization. No machine-learning model is used.

## Important Note
The source file contains SLB market data rather than normal TCS cash-market share-price history. Multiple SLB settlement series can be traded on the same date, so the project aggregates activity at the daily level where appropriate.

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
- 7-day moving averages
- Highest-volume trading days
- Highest-value trading days
- Correlation between market activity measures
- Distribution of weighted SLB prices

## Weighted Average Price
Because several SLB series may trade on the same day, the project calculates:

Weighted Average Price = Total Traded Value / Total Traded Quantity

This gives a simple daily measure of the average traded SLB price across active series.

## How to Run in Google Colab
1. Upload `TCS_SLB_Market_Analysis.ipynb`.
2. Run the notebook from the first cell.
3. When prompted, upload `Quote-SLB-TCS-EQ-9-03-2026-to-9-09-2026.csv`.
4. Run all cells in order.

## Skills Demonstrated
- Financial data cleaning
- Time-series data handling
- Pandas groupby and aggregation
- NumPy calculations
- Market activity analysis
- Moving averages
- Correlation analysis
- Financial data visualization with Matplotlib

## Future Improvements
- Add cash-market TCS share-price data.
- Compare SLB activity with TCS price movements.
- Compare SLB activity across multiple companies.
- Analyze individual settlement series in more detail.
