# Mean Reversion Signals on DOGE/USDT

A small research notebook comparing simple mean-reversion signals on daily DOGE/USDT data from Binance.

## What's inside
- **Data**: daily klines pulled from the Binance public API (`get_crypto_data`), with a cached snapshot in `dogecoin_daily_20250603.csv` so the notebook runs offline
- **Signals**: 200-day moving average, MA20/MA200 crossover, Bollinger Bands (20-day, 2σ), RSI, and a combined signal
- **Backtest**: long/flat backtest with signals lagged one bar to avoid look-ahead
- **Evaluation**: total and annualized return, Sharpe, max drawdown, trade statistics, and equity-curve plots per signal

## Run
```bash
pip install pandas numpy matplotlib requests
jupyter notebook mean_reversion_model.ipynb
```

This is an exploratory study, not a production strategy.
