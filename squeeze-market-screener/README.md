# squeeze-market-screener

Codex skill for scanning US and Taiwan markets with the Squeeze Momentum workflow.

## Install

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo mylin102/squeeze-us-skill \
  --path squeeze-market-screener
```

Restart Codex after installation so the new skill is loaded.

## Example Commands

```bash
squeeze-us scan --export --plot --notify
squeeze-tw scan --export --plot --notify
squeeze-us analyze --ticker NVDA
```
