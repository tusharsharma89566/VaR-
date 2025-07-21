# VaR-

## Portfolio Value at Risk Assessment Using Yahoo Finance Data

VaR- is a Python-based tool for assessing the Value at Risk (VaR) of financial portfolios using historical data from Yahoo Finance. It helps investors and analysts to estimate potential losses in their portfolios over a specified period and confidence interval.

---

## Features

- **Fetch historical price data from Yahoo Finance**
- **Calculate portfolio returns and statistics**
- **Compute Value at Risk (VaR) using methods like historical simulation, variance-covariance, and Monte Carlo simulation**
- **Visualize risk metrics and portfolio performance**
- **Flexible portfolio input (CSV, manual entry, etc.)**

---

## Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/tusharsharma89566/VaR-.git
    cd VaR-
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

---

## Usage

1. **Prepare your portfolio file**

    Create a CSV file (e.g., `portfolio.csv`) with your holdings:
    ```
    Ticker,Allocation
    AAPL,0.3
    MSFT,0.4
    TSLA,0.3
    ```

2. **Run the VaR analysis**
    ```bash
    python var.py --portfolio portfolio.csv --method historical --confidence 0.95 --window 252
    ```

    - `--portfolio`: Path to your portfolio file
    - `--method`: VaR calculation method (`historical`, `var-covar`, `monte-carlo`)
    - `--confidence`: Confidence level (e.g., 0.95 for 95%)
    - `--window`: Number of historical days to use

3. **Example Output**

    ```
    Portfolio VaR (95% confidence, 1-day): $1,500
    ```

---

## File Structure

```
├── var.py
├── requirements.txt
├── README.md
├── portfolio.csv
```

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements and bug fixes.

---

## License

This project is licensed under the MIT License.
