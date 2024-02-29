# Trading_at_the_close - Kaggle Challenge

This project explores predicting closing price movements of Nasdaq-listed stocks using data from the daily ten-minute closing auction on the NASDAQ stock exchange. The primary goal is to forecast future price movements relative to a synthetic index. This analysis plays a crucial role in enhancing market efficiency, especially during the final minutes of trading, which are often marked by heightened volatility.

## Dataset variables

- stock_id: Unique identifier for the stock
- date_id: Unique identifier for the date
- imbalance_size: Unmatched amount at the current reference price (USD)
- imbalance_buy_sell_flag: Indicator of auction imbalance direction
- reference_price: Near price bounded between the best bid and ask price
- matched_size: Amount that can be matched at the current reference price (USD)
- far_price: Crossing price for maximizing shares matched based on auction interest
- near_price: Crossing price for maximizing shares matched including continuous market orders
- bid/ask_price: Most competitive buy/sell level in the non-auction book
- bid/ask_size: Dollar notional amount on the most competitive buy/sell level in the non-auction book
- wap: Weighted average price in the non-auction book
- seconds_in_bucket: Seconds elapsed since the start of the day's closing auction
- target: 60-second future move in the weighted average price of the stock less the synthetic index move

## Data preparation pipeline 

- Data collection 
- Data Profiling 
  - Understand the data characteristics 
  - Identify missing values and anomalies 
  - Collecting statistics 
  - Metadata exploration 
- Data Cleaning 
  - Impute or remove missing values 
- Data transformation  
  - Encoding
  - Create new features 
  - Normalize and scale 
- Feature selection 
  - Reduce dimensionality 
- Data splitting 
- Feature extraction 
