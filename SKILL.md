# squeeze-us-screener

## Purpose
This skill should be used when the user wants to scan the US stock market for technical patterns, specifically the Squeeze Momentum indicator, and analyze high-quality assets from major indices (S&P 500, NASDAQ 100, DJI, SOX). It automates the end-to-end workflow from ticker discovery to report generation and performance tracking.

## When to Use This Skill
- Scanning for "Squeeze On" or "Squeeze Fired" setups in the US market.
- Identifying advanced patterns like "Houyi Shooting Sun" or "Whale Trading".
- Filtering stocks by fundamental metrics (Market Cap, Volume, Value Score).
- Managing and reviewing the active 25-stock tracking list in recommendations.csv.
- Generating automated market summary reports and technical charts.

## Core Capabilities
1. **Dynamic Ticker Discovery**: Automatically fetches the latest constituents from S&P 500, NASDAQ 100, DJI, and SOX via Wikipedia (~520+ stocks).
2. **Squeeze Momentum Analysis**: Calculates Bollinger Bands and Keltner Channels to identify volatility compression and momentum direction.
3. **Pattern Recognition**: Detects classic TTM Squeeze, price-extreme reversal (Houyi), and multi-timeframe alignment (Whale).
4. **Automated Reporting**: Generates high-quality Markdown reports and technical charts using Plotly/Matplotlib.
5. **Portfolio Performance Tracking**: Maintains a clean, 25-item recommendation list to track historical accuracy and price returns.

## Usage Instructions
- **Run Full Scan**: `squeeze scan --export --plot --notify`
- **Filter by Market Cap**: `squeeze scan --min-mkt-cap 10` (Stocks > 10B USD)
- **Check Specific Ticker**: `squeeze analyze --ticker TSLA`
- **Update Tracking List**: Automatically handled during scan, restricted to latest 25 picks.

## Metadata
- **Author**: mylin102
- **Version**: 1.0.0
- **Triggers**: scan US stocks, analyze squeeze momentum, check stock recommendations, run squeeze scanner
