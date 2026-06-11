---
name: quant-real-factor-7d-time-series-ranked-upper-breakout
description: Use when computing the 7D Time-Series Ranked Upper Breakout factor from user-supplied real OHLCV data or reviewing its bundled real-data validation metrics.
metadata:
  organization: QuantSkills
  organization_url: https://github.com/quantskills
  repository: skill-quant-factor-directional-alpha
  repository_url: https://github.com/quantskills/skill-quant-factor-directional-alpha
  collection: directional-alpha
  factor_id: R372
  category: Breakout
---

# 7D Time-Series Ranked Upper Breakout

Use this Skill to compute `7日时序排名上轨突破` / `7D Time-Series Ranked Upper Breakout` from caller-provided OHLCV data.

## Workflow

1. Load a `pandas.DataFrame` with `open`, `high`, `low`, `close`, `volume`; include `date` and `symbol` for cross-sectional research.
2. Call `scripts/factor.py::compute_factor(df)` to compute the factor column.
3. Call `generate_signals(df)` for a simple rank-based long/short signal.
4. Review `validation_real/report.md` before using the factor in a model.

## Runtime Contract

- Framework-neutral Python: `pandas` and `numpy`.
- The caller owns data vendor, universe, calendar, costs, slippage, and execution modeling.
