# Black-Litterman Model on S&P/TSX 60 Index

This project applies the Black-Litterman model to the Canadian S&P/TSX 60 index using **Bloomberg Python API** for **data extraction** and **financial modeling**.

## Features

- Web scraping S&P/TSX 60 constituents (non-Wikipedia source)
- Historical data download via Bloomberg API (2020–2025)
- Correlation & covariance matrix generation
- Market-cap weighted portfolio construction
- Black-Litterman expected return derivation
- Portfolio adjustments based on active views
- Heatmaps and pie charts for visual insights

## Active Views Modeled

1. Shopify to outperform Rogers by 5%
2. Loblaw expected to return 1% more than its 5-year average

## Tools & Libraries

- Python 3.x
- Bloomberg Python API (`blpapi`)
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `cvxpy` or `pyportfolioopt` for optimization
- `requests`, `bs4` for web scraping

## Structure

- `src/` – Core logic and model implementation
- `notebooks/` – Jupyter Notebook walkthrough
- `data/` – Raw and processed data (if shareable)
- `plots/` – Charts and heatmaps

## License

MIT License
