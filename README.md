# AI agent and automation platform pricing data

Open data from [gravity.fast](https://gravity.fast/), updated 2026-09-15.

- `pricing/index.json`, `pricing/index.csv`: current free tier, starting paid price, billing unit and last price change for 16 tools, verified 2026-09-15. Human-readable: [AI agent pricing index](https://gravity.fast/blog/ai-agent-pricing-index/).
- `pricing/history.json`: dated plan-price periods per tool from monthly Wayback Machine snapshots since January 2024, each with its archived source URL. Per-tool pages: `https://gravity.fast/blog/<tool>-pricing-history/`.
- `pricing/catalog.json`: the curated source of the index, with a confidence flag per row and a dated change log.
- `statistics/`: sourced statistics tables behind the [AI agent adoption statistics](https://gravity.fast/blog/ai-agent-adoption-statistics-2026/) hub and its sibling pages (publisher, date, method, URL per row).

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, republish it, build on it. Attribution: "Gravity, https://gravity.fast/blog/ai-agent-pricing-index/" with a link.

## Method

A script snapshots each vendor's pricing page (live, rendered for JavaScript pages) and the Wayback Machine's monthly captures, extracts the plan prices, and records a new period when the set changes. A person checks the change against the live page before it enters the index. Rows marked `page-figure` carry a figure the page shows without an unambiguous plan name; `not-published` means the page shows no price. Corrections: open an issue or email hello@gravity.fast.
