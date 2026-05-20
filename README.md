# Pivotwise

A pivot planner agent for the Social Links API - given a partial investigation graph, it ranks the next 5 highest yield transform invocations by expected information gain, with a Spanish/Portuguese native UI for LATAM channel partners.

## Why This Exists

Social Links' own Crimewall page headlines "AI powered link analysis and automation." Under the marketing, the actual AI moments inside an investigation today are mostly classifier level (image recognition, sentiment, OCR) - not the agentic layer that decides which of the 1,500 methods to fire next given a partially built graph. The YouTube tutorials walk human analysts through pivot heuristics one by one; that institutional knowledge does not live in the product.

## What It Builds

- Replays synthetic `social` and `links` cases against the project's evidence rules.
- Scores `social_coverage`, `links_risk`, and `crimewall_precision` so regressions are visible in CSV and JSON.
- Plants `social drift` and `links gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `pivotwise` without hosted services.

## Local Run

```bash
uv sync
uv run pivotwise all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/domain_rubric.json`
- `outputs/failure_matrix.md`
- `outputs/trace_graph.mmd`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://sociallinks.io/products/sl-crimewall
- https://sociallinks.io/products/sl-professional
- https://sociallinks.io/products/sl-private-platform
- https://sociallinks.io/channel-partner-program
- https://github.com/SocialLinks-IO
- https://github.com/SocialLinks-IO/telegram-similar-channels
- https://github.com/SocialLinks-IO/sociallinks-api
- https://www.maltego.com/transform-hub/social-links-pro/
- https://docs.maltego.com/en/support/solutions/articles/15000054072-social-links-pro
- https://www.youtube.com/playlist?list=PL7DhkxY3DMy17SBblDHSzU0j5rRJ36iQW

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
