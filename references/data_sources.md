# Data Source Rules

Use real, traceable data for factor validation and BACKTEST execution.

## Required Provenance

Record the following in `manifest.json` and the HTML reports:

- Data provider or file source.
- Local file path, URL, database path, or BACKTEST config source.
- Symbols/universe.
- Sample period.
- Frequency.
- Adjustment rules.
- Data availability timestamp or publish-time assumption when relevant.
- Missing-value handling.

## Prohibited Data

Do not use synthetic, mock, or randomly generated market data to prove factor effectiveness.

A fixed-seed random factor is allowed only as a negative-control baseline on the same real return data used by the target factor.

## Insufficient Data

If data cannot support the report's factor test:

- Keep the required report section.
- State the concrete blocker in Chinese.
- Mark the conclusion as `inconclusive`.
- Create or update `failure_report.md` if the project cannot proceed.
