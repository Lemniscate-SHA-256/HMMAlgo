# HMM-Based Asset Analysis

This project analyzes financial assets using a Hidden Markov Model (HMM) to identify different market regimes and patterns. The analysis includes calculating daily returns, rolling volatility, and volume changes, and visualizing the hidden states identified by the HMM.

## Features

- Fetches historical asset data using yfinance
- Calculates daily returns, rolling volatility, and volume changes
- Cleans the data by handling NaN and infinite values
- Standardizes the data using StandardScaler
- Fits a Gaussian HMM model with 4 hidden states
- Predicts hidden states and adds them to the original data
- Plots hidden states against asset prices for visualization

## Installation

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/your-repo/hmm-based-asset-analysis.git
   cd hmm-based-asset-analysis
   ```

2. **Install Dependencies**:
   ```sh
   pip install -r requirements.txt
   ```

## Usage

To run the analysis, use the following command:

```sh
python hmmAlgo.py --ticker <TICKER_SYMBOL> --start_date <START_DATE> --end_date <END_DATE> --plotter <PLOTTER_TYPE>
```

Replace `<TICKER_SYMBOL>`, `<START_DATE>`, `<END_DATE>`, and `<PLOTTER_TYPE>` with appropriate values. For example:

```sh
python hmmAlgo.py --ticker AAPL --start_date 2020-01-01 --end_date 2021-01-01 --plotter line
```

## Example Output

After running the analysis, you will see visualizations of hidden states against asset prices.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

I would like to thank the contributors of the following libraries and tools that made this project possible:
- [yfinance](https://github.com/ranaroussi/yfinance)
- [hmmlearn](https://github.com/hmmlearn/hmmlearn)
- [matplotlib](https://matplotlib.org/)
- [scikit-learn](https://scikit-learn.org/)
