---
name: quant-factor-directional-alpha
description: Use when an agent needs a verified library of directional OHLCV alpha
  factor Skills for trend, breakout, reversal, channel-position, or price-direction
  research across A-share and US equity samples.
quantSkills:
  project_type: skill
  category: factor
  tags:
  - alpha-factor
  - directional
  - ohlcv
  - trend
  - breakout
  platforms:
  - claude-code
  - codex
  - openclaw
  - cursor
  status: stable
  validation_level: verified
  maintainer_type: official
  summary_zh: 方向类因子库：296 个独立 OHLCV 因子 Skill，真实行情验证 296/296 全部通过。
  summary_en: Directional OHLCV alpha factor library with 296 trend, breakout, reversal,
    and channel-position factor Skills validated on real market data.
  license: GPL-3.0
---

# Quant Factor Directional Alpha

Use this skill when an agent needs to select, inspect, or apply directional OHLCV alpha factor Skills from this repository.

## Workflow

1. Read [README.md](README.md) for the repository-level inventory, validation scope, and market sample.
2. Use `factor_index.json` to locate the relevant factor family or individual factor directory.
3. Open the selected factor folder under the factors directory and follow its local instructions before writing or running code.
4. Treat validation metrics as historical research evidence, not investment advice. Re-run validation when the universe, time range, data vendor, or execution assumptions change.

## Scope

This repository focuses on price direction, trend continuation, breakout, reversal, and channel-position signals built from OHLCV data.
