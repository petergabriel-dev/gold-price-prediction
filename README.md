# Gold Prices Prediction

A machine learning project for analyzing and predicting gold prices using historical data from Binance.

## Project Overview

This project fetches historical gold price data (PAXGUSDT) from the Binance API, performs data analysis, and prepares the foundation for building predictive models.

## Current Progress

### ✓ Completed
- **Data Fetching**: Retrieve 180 days of historical 4-hour candlestick data from Binance
- **Data Processing**: 
  - Parse and structure raw klines data into a pandas DataFrame
  - Convert timestamps from milliseconds to datetime objects
  - Cast OHLCV columns to appropriate float types
- **Data Validation**:
  - Time continuity checks for data gaps
  - Extreme price movement detection (>10% changes)
  - Basic statistical analysis (mean, min, max, price range)
- **Data Export**: Save processed data to CSV for further analysis

### 📊 Data Pipeline
1. Initialize Binance client
2. Fetch historical klines (PAXGUSDT, 4h interval, 180 days)
3. Transform raw data into structured DataFrame
4. Validate data quality
5. Export to `gold_price_data.csv`

### 📈 Current Metrics
- **Symbol**: PAXGUSDT (PAX Gold in USDT)
- **Interval**: 4-hour candles
- **Period**: Last 180 days
- **Data Points**: ~1,080 candles (approx.)

## Files
- `main.ipynb` - Main Jupyter notebook with data pipeline and analysis
- `gold_price_data.csv` - Exported historical price data

## Next Steps (Planned)
- [ ] Exploratory Data Analysis (EDA) visualizations
- [ ] Feature engineering (moving averages, RSI, MACD, etc.)
- [ ] Train/test data splitting
- [ ] Build and train predictive models
- [ ] Model evaluation and backtesting

## Requirements
- pandas
- python-binance
- numpy

## Usage
Run cells sequentially in `main.ipynb` to:
1. Connect to Binance
2. Fetch historical data
3. Process and validate
4. View statistics and export data

---
**Status**: Data collection and validation phase ✓
**Last Updated**: November 16, 2025