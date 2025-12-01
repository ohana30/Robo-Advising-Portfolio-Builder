# Robo-Advising-Portfolio-Builder

Robo-Advising Portfolio Builder — AFM 127 (Market Meet Winner)

Overview:

This project was completed for AFM 127 – Robo-Advising Challenge.
Our team designed a Python-based robo-advisor that automatically constructs a diversified equity portfolio following strict competition rules. The portfolio was tested on real market data over a one-week period using a secret list of stock tickers.
Our group selected the Market Meet strategy, aiming to achieve a total return closest to the benchmark average (the mean return of the TSX Composite and S&P 500).

Result: Won the Market Meet category in the class case competition.

Project Goals: 
- Build a self-adjusting portfolio generator using Python (no hardcoding).
- Handle any random ticker list provided at runtime and ensure full rule compliance.
- Achieve performance closest to the competition benchmark.
Output the final portfolio in both DataFrame and CSV formats.

Repository Structure

Technologies & Tools Used: 
- Python (pandas, numpy)
- Jupyter Notebook
- Data cleaning & filtering
- Portfolio optimization logic

Features: 
- Automated Stock Filtering
- Removes securities with <5,000 average daily volume
- Ensures only US + Canadian equities
- Filters invalid tickers or missing data
  
Portfolio Construction:
- Selects 10–25 stocks
- Enforces minimum/maximum weights
- Market-cap mix: 1 large-cap & 1 small-cap
- Total portfolio value ≈ $1,000,000 CAD
- Uses fractional shares to meet target allocation

Benchmarks portfolio returns against:
- S&P 500
- TSX Composite
- Computes the benchmark’s simple average return
- Measures performance distance from benchmark (Market Meet goal)
  
Final Outputs:
Portfolio_Final DataFrame (Ticker, Price, Shares, Weight, Value)
Stocks_Group_XX.csv (Ticker, Shares)
Markdown analysis and summary

Our Market Meet strategy focused on:
- Selecting stable, moderate-volatility stocks that historically tracked the benchmark closely
- Balancing sectors to reduce outlier performance
- Weighting mid-cap and large-cap stocks slightly higher to smooth short-term deviations
- Limiting exposure to high-volatility small-caps except to satisfy the required small-cap rule
-This approach produced returns very close to the benchmark during the one-week evaluation period — resulting in a 1st place finish.

** Academic Integrity Note **
This project was completed following AFM 127 guidelines, with no AI usage in the code itself.

This README is for GitHub documentation only.
