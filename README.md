# Black-Litterman Model on S&P/TSX 60 Index

This project applies the Black-Litterman model to the Canadian S&P/TSX 60 index using **Bloomberg Python API** for **data extraction** and **financial modeling**.

## Features

- Web scraping S&P/TSX 60 constituents (from the Globe and Mail website(non-Wikipedia source): https://www.theglobeandmail.com/investing/markets/indices/TXSX/components/)
- Historical data download via Bloomberg API (2020–2025)
- Correlation & covariance matrix generation
- Market-cap weighted portfolio construction
- Black-Litterman expected return derivation
- Portfolio adjustments based on active views
- Heatmaps and pie charts for visual insights

## Active Views Modeled

assume that you are a portfolio manager that has the following active views:

1.	Shopify will outperform Rogers by 5%.
2.	Return on Loblaw Companies Limited will be 1% higher than its average over the most recent 5-year period (the May 16, 2020 - May 16, 2025)

Calculate the Black-Litterman optimal portfolios:
1.	Using the first view only.
2.	Using the second view only.
3.	Using both views.

## Tools & Libraries

- Python 3.x
- Bloomberg Python API (`blpapi`, `xbbg`)
- `pandas`, `numpy`, `matplotlib`, `seaborn`, `yfinance`
- `requests`, `bs4`, `selenium` for web scraping

## Structure

- `src/` – Core logic and model implementation
- `notebooks/` – Jupyter Notebook walkthrough
- `data/` – Raw and processed data (if shareable)
- `plots/` – Charts and heatmaps

## License

MIT License
