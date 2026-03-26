# squeeze-market-screener

## Purpose
This skill should be used to scan and analyze both US and Taiwan stock markets for technical patterns, specifically the Squeeze Momentum indicator. It automates ticker discovery from major indices (S&P 500, NASDAQ 100, DJI, SOX for US; TWSE, TPEx, Emerging for Taiwan) and manages performance tracking.

## When to Use This Skill
- Scanning for "Squeeze On" or "Squeeze Fired" setups in US or Taiwan markets.
- Identifying advanced patterns like "Houyi Shooting Sun" or "Whale Trading".
- Filtering stocks by fundamental metrics (Market Cap, Volume, Value Score).
- Managing a high-signal tracking list restricted to the latest 25 recommendations per market.
- Generating automated market summary reports and technical charts.

## Core Capabilities
1. **Multi-Market Ticker Discovery**: 
   - **US**: Dynamic fetching of S&P 500, NASDAQ 100, DJI, and SOX constituents.
   - **Taiwan**: Full coverage of Listed (TWSE), OTC (TPEx), and Emerging (EMG) stocks via ISIN system.
2. **Squeeze Momentum Engine**: Unified calculation of Bollinger Bands and Keltner Channels to identify volatility break-outs.
3. **Smart Pattern Recognition**: Detection logic for TTM Squeeze, Houyi (extreme reversal), and Whale (multi-timeframe) trading.
4. **Automated Reporting**: Generation of Chinese/English Markdown reports and visualization charts.
5. **Intelligent Performance Tracking**: Maintains a clean 25-item tracking database to evaluate signal accuracy over time.

## Usage Instructions
- **Scan US Market**: `squeeze-us scan --export --plot`
- **Scan Taiwan Market**: `squeeze-tw scan --export --plot`
- **Filter by Market Cap (US)**: `squeeze-us scan --min-mkt-cap 10`
- **Check Specific Ticker**: `squeeze-us analyze --ticker NVDA` or `squeeze-tw analyze --ticker 2330.TW`

## Metadata
- **Author**: mylin102
- **Version**: 1.1.0
- **Triggers**: scan US stocks, scan Taiwan stocks, analyze squeeze momentum, check stock recommendations, run market scanner, 掃描台股, 掃描美股
