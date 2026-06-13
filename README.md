# sgrm-regime-feed

Public JSON feed for SGRM WSP put-writer dashboards.

This repo serves three files via GitHub Pages:
- `regime.json` — latest seven-lens market regime read
- `daily_plan.json` — latest daily plan
- `meta.json` — feed metadata

Updated automatically by the operator VM cron via `jobs/publish_regime.sh`.

Friend dashboards consume these endpoints by setting "Shared regime feed URL"
to `https://chattime.github.io/sgrm-regime-feed/regime.json` in their SGRM
WSP HTML settings.
