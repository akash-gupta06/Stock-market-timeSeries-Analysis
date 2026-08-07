# Time Series Stock Market Analysis
 
A Python project analyzing 5 years of stock price data for 4 major companies — **Apple, Amazon, Google, and Microsoft** — to understand risk, returns, and price trends.
 
## What This Project Does
 
- Finds which stock is the **safest** (least volatile) to invest in
- Finds which stock gave the **highest returns** over 5 years
- Simulates how ₹1,00,000 invested would have grown over time
- Spots each stock's **worst crash days** (biggest single-day losses)
- Tracks **price trends** using 20-day and 50-day moving averages
- Checks if any **month of the year** historically gives better returns
## Dataset
 
Daily stock data (Open, High, Low, Close, Volume) for AAPL, AMZN, GOOG, and MSFT, spanning 2013–2018 (~4,750 rows).
 
## How It Works
 
1. **Cleaned the data** — fixed date formats, checked for missing/duplicate values, sorted by date
2. **Calculated daily returns** (% change in closing price each day)
3. **Measured risk** using the standard deviation of daily returns — higher = more volatile
4. **Calculated cumulative returns** to see total growth over the full period
5. **Found the worst days** for each stock using the lowest daily returns
6. **Added moving averages** to smooth out price and reveal the overall trend
7. **Grouped returns by month** to check for seasonal patterns
## Tools Used
 
Python, Pandas, NumPy, Matplotlib, Plotly
 
## Key Results
 
| Question | Answer |
|---|---|
| Safest stock (lowest risk) | Google |
| Best returns overall | Amazon (~5.4x growth) |
| ₹1,00,000 in Amazon grew to | ~₹5.4 lakh |
 
## What Could Be Added Next
 
- Test a simple trading strategy (buy/sell based on moving average crossovers) and see if it beats just holding the stock
- Add a risk-adjusted return metric (like Sharpe Ratio) for fairer comparison
- Try this same analysis on more stocks or on futures/derivatives data
