# Machine Learning for Bitcoin Trading

This repository demonstrates how to apply machine learning to develop a trading strategy using Bitcoin daily data. The approach leverages predictive modeling to generate trading signals based on historical price movements and external indicators.

## Features
- **Data Collection**: Incorporates Bitcoin trading volume, Google Trends data ([source](https://github.com/qztseng/google-trends-daily)), and hashrate data from CoinGecko.
- **Feature Engineering**: Constructs predictive features from historical data.
- **Machine Learning Modeling**: Trains a model to predict price movements.
- **Trading Strategy**: Enters a trade when the predicted return is positive and exits at the day's close.
- **Backtesting**: Evaluates strategy performance using historical data.
- **Visualization**: Provides insights into model predictions and trading performance.

## Installation
Ensure you have the required dependencies installed:

```bash
pip install pandas numpy scikit-learn matplotlib yfinance vectorbt
```

## Usage
Run the Jupyter Notebook to train the model and evaluate the strategy:

```bash
jupyter notebook Bitcoin_machine_learning_strategy.ipynb
```

## Data Sources
- **Bitcoin Trading Volume**: Extracted from Yahoo Finance via `yfinance`.
- **Google Trends Data**: Retrieved from [this repository](https://github.com/qztseng/google-trends-daily).
- **Bitcoin Hashrate**: Obtained from CoinGecko API.

## Strategy Logic
1. **Train the Model**: Uses historical data to predict Bitcoin's daily return.
2. **Generate Trading Signals**: Enter a trade when the model predicts a positive return.
3. **Exit Criteria**: Exit at the end of the trading day.
4. **Backtesting**: Evaluate performance based on past data.

## Results
- **Data visualization** for better insight into Bitcoin trends.
- **Model evaluation** using accuracy metrics.
- **Backtesting outcomes** showing profitability and risk assessment.

## Contributing
Feel free to fork this repository and submit pull requests for improvements.

