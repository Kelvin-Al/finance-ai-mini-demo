# Project Plan

## Project Goal

Develop a clear and reproducible research workflow for comparing three familiar asset classes represented by the ETFs SPY (US equities), TLT (long-term US Treasury bonds), and GLD (gold). The workflow will use risk-and-return metrics to support a structured, data-driven comparison.

## Available Data

The file `data/etf_snapshot.csv` contains a small synthetic dataset with one row per ETF. The dataset is **synthetic teaching data** — it is not live or historical market data. The six columns are:

| Column | Meaning |
|---|---|
| `ticker` | ETF identifier |
| `asset_class` | Broad asset type |
| `expected_return_pct` | Illustrative annual return assumption (%) |
| `volatility_pct` | Illustrative annual variability (%) |
| `max_drawdown_pct` | Illustrative peak-to-trough loss (%) |
| `expense_ratio_pct` | Illustrative annual fund fee (%) |

A data dictionary (`data/data_dictionary.md`) describes each column and its limitations.

## Expected Final Deliverable

A Markdown report that compares SPY, TLT, and GLD on expected return, volatility, max drawdown, and expense ratio. The report will include summary metrics and a plain-language interpretation of the trade-offs among the three asset classes.

## Three Project Milestones

1. **Project setup and planning** — Create this project plan, review the data dictionary and CSV structure, and confirm the scope.
2. **Exploratory analysis** — Compute summary statistics (mean, range, ranking) for each metric and produce a comparison table or chart.
3. **Interpretation and write-up** — Draft the final report that explains the risk-return profile of each ETF and highlights the key trade-offs, and discuss the limitations of the synthetic data.

## One Data Limitation

All numeric values in the dataset are synthetic teaching assumptions. They are not current market quotations, verified historical estimates, or forecasts. The dataset also omits correlations among the assets, taxes, transaction costs, liquidity, currency exposure, and investor-specific constraints, so any conclusions drawn from it are illustrative only.

## Next Action

Review this plan and confirm it matches the repository scope. If approved, save the file with Git under `artifacts/t1/project-plan.md` and proceed to the exploratory analysis milestone.