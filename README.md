# Stock Price Analysis

Comparative equity price visualization for Tesla (TSLA) and CrowdStrike (CRWD) over summer 2024 (June–August). Focuses on data cleaning, date-range filtering, and interactive charting.

## Notebook

`stock_visualization.ipynb` — loads historical OHLCV CSVs, converts and sorts dates, filters to the summer window, and plots individual and combined closing price line charts using Plotly.

## Data

Expects two CSV files in the working directory:
- `Tesla.csv`
- `Crowdstrike.csv`

Each should contain at minimum: `date`, `close` columns. Historical price data can be downloaded from Yahoo Finance or any standard market data provider.

## Stack

- **pandas** — date parsing, sorting, filtering
- **Plotly** — interactive line charts

## Setup

```bash
conda create -n stocks pandas plotly ipykernel python -c conda-forge -y
conda activate stocks
```
