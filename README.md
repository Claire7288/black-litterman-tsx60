# Black-Litterman Model on S&P/TSX 60 Index

This project implements the **Black-Litterman asset allocation model** on the **S&P/TSX 60 Index**, combining financial theory with real market data using Python and the Bloomberg Terminal API.

It is designed to help finance students and professionals understand how to integrate market equilibrium returns with personal investment views using real-world Canadian equity data.

---

## Overview

This project is divided into two key stages:

1. **Ticker Scraping**  
   - Scrapes the latest list of TSX 60 constituents **from The Globe and Mail website** (not Wikipedia).
   - Uses `selenium` and `webdriver` to navigate and extract tickers dynamically.

2. **Data Download & Black-Litterman Modeling**  
   - Downloads daily stock price and market cap data using the **Bloomberg Python API (`blpapi` and `xbbg`)**.
   - Computes covariance and correlation matrices, constructs the market-cap weighted portfolio, and applies the Black-Litterman model with and without active views.
   - Visualizes correlation heatmaps, market weight pie charts, and weight shifts from views.

---

## Active Views Modeled

As a portfolio manager, we assume the following active investment views:

1. **Shopify will outperform Rogers by 5%.**  
2. **Loblaw's return will be 1% higher than its average over the past 5 years (2020–2025).**

Using these views, we generate three optimized portfolios:
- Based on View 1 only
- Based on View 2 only
- Based on both views combined

---

## Visual Outputs

- **Correlation matrix** (Seaborn heatmap)
- **Market cap weights** (Pie chart)
- **Portfolio weight changes** (Bar chart comparison)

---

## Tools & Libraries

- Python 3.x
- `blpapi`, `xbbg` – Bloomberg API access
- `selenium`, `bs4`, `requests` – Web scraping
- `pandas`, `numpy`, `matplotlib`, `seaborn` – Data analysis & plotting
- `yfinance` 

---

## 📁 Project Structure
├── src/
│   ├── scrape_tsx60_tickers.py    # Web scraping from Globe and Mail
│   └── black_litterman_model.py   # Data download, modeling, visualization
├── notebooks/
│   └── walkthrough.ipynb          # Step-by-step notebook version
├── data/                          # Saved or shared price/cap data
├── plots/                         # Output charts and heatmaps
└── README.md

---

## Requirements & Access Notes

- To **run the Black-Litterman model**, your machine must:
  - Have **access to a Bloomberg Terminal**
  - Be configured with `blpapi` and valid Bloomberg credentials
- The scraping module (`scrape_tsx60_tickers.py`) does **not require Bloomberg**.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Contributions

Pull requests are welcome! If you want to add new views, extend the model, or enhance visuals, feel free to contribute.

---
