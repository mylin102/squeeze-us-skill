# Squeeze Market Screener Skill (US & TW)

This skill brings the power of the **Squeeze Stock Screener** for both US and Taiwan markets directly into your CLI. It facilitates the discovery of high-momentum trading opportunities across the world's most important indices.

## Features
- **Global Coverage**: 
  - **US**: S&P 500, NASDAQ 100, DJI, SOX (~520+ stocks).
  - **Taiwan**: TWSE, TPEx, and Emerging stocks (~1800+ stocks).
- **Efficient Tracking**: Automatically manages and limits the recommendation list to the latest 25 high-signal stocks per market.
- **Advanced Patterns**: Includes Squeeze, Houyi Shooting Sun, and Whale Trading detection.

## Quick Start
```bash
# Scan Taiwan market top picks
squeeze-tw scan --limit 100 --plot --export

# Scan US market tech stocks
squeeze-us scan --limit 50 --plot --export
```
