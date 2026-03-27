# Squeeze Market Screener Skill (US & TW)

This repository contains the installable Codex skill in the `squeeze-market-screener/` directory.

## Install

Use the standard skill installer against the skill subdirectory:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo mylin102/squeeze-us-skill \
  --path squeeze-market-screener
```

If your environment still targets the legacy `master` branch explicitly, this also works:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo mylin102/squeeze-us-skill \
  --ref master \
  --path squeeze-market-screener
```

Restart Codex after installation so the new skill is loaded.

## Features
- **Global Coverage**:
  - **US**: S&P 500, NASDAQ 100, DJI, SOX (~520+ stocks).
  - **Taiwan**: TWSE, TPEx, and Emerging stocks (~1800+ stocks).
- **Pro Reporting**: Generates HTML email reports with technical chart attachments automatically.
- **Efficient Tracking**: Automatically manages and limits the recommendation list to the latest 25 high-signal stocks per market.
- **Advanced Patterns**: Includes Squeeze, Houyi Shooting Sun, and Whale Trading detection.

## Quick Start

```bash
# Scan Taiwan market top picks with HTML email & charts
squeeze-tw scan --plot --export --notify

# Scan US market tech stocks with HTML email & charts
squeeze-us scan --plot --export --notify
```
