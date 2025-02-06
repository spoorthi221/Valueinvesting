# Stock Portfolio Optimization with Machine Learning

This project implements a comprehensive stock portfolio optimization strategy that combines traditional financial metrics with machine learning approaches. The system analyzes stocks from major indices and creates optimized portfolios using multiple methodologies.

## Features

### 1. Data Collection and Processing
- Fetches historical price data and financial metrics using yfinance
- Processes fundamental data (PE ratio, PB ratio, Revenue Growth, etc.)
- Calculates technical indicators (RSI, MACD, Moving Averages)

### 2. Traditional Analysis
- Implements value-based stock screening
- Calculates fundamental ratios and growth metrics
- Creates rankings based on multiple financial factors
- Position sizing based on risk metrics

### 3. Machine Learning Enhancement
- Uses Random Forest and Gradient Boosting models
- Features include both technical and fundamental indicators
- Cross-validation for model evaluation
- Ensemble approach for prediction stability

### 4. Portfolio Construction
- Three portfolio construction methods:
  - Traditional (based on financial metrics)
  - ML-Enhanced (using machine learning predictions)
  - Hybrid (combining both approaches)
- Sector diversification rules
- Risk management constraints
- Dynamic position sizing

### 5. Performance Analysis
- Backtest results with key metrics:
  - Annual Returns
  - Volatility
  - Sharpe Ratio
  - Maximum Drawdown
- Portfolio comparison tools
- Risk-adjusted return analysis

## Project Structure

```
├── setup.py                  # Initial setup and imports
├── data_collection.py        # Data fetching and processing
├── metrics_calculation.py    # Financial metrics calculation
├── ranking_system.py        # Traditional ranking implementation
├── ml_analysis.py           # Machine learning models
├── visualization.py         # Portfolio visualization tools
└── portfolio_comparison.py  # Comparison of different strategies
```

## Requirements

```python
yfinance==0.2.18
pandas==2.0.0
numpy==1.23.5
scikit-learn==1.2.2
matplotlib==3.7.1
ta==0.10.2
```

## Key Results

1. Traditional Portfolio:
   - Annual Return: 15.1%
   - Volatility: 24.4%
   - Sharpe Ratio: 0.617

2. ML-Enhanced Portfolio:
   - Annual Return: 5.5%
   - Volatility: 20.8%
   - Sharpe Ratio: 0.264

3. Key Findings:
   - 30% overlap between traditional and ML approaches
   - ML portfolio shows better risk management
   - Traditional portfolio delivers higher returns
   - Hybrid approach balances risk and return

## Usage

1. Clone the repository:
```bash
git clone https://github.com/spoorthi221/Valueinvesting.git
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. Run the analysis:
```bash
python main.py
```

## Future Improvements

1. Add more technical indicators
2. Implement real-time data updates
3. Include transaction costs
4. Add more ML models
5. Implement dynamic rebalancing

## Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

MIT

## Contact

Spoorthi Veeresh Kumar
spoorthiv20@gmail.com

## Acknowledgments

- Financial data provided by Yahoo Finance
- Technical analysis features from ta library
- Machine learning implementation using scikit-learn
