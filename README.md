# Pivotwise

A pivot planner agent for the Social Links API - given a partial investigation graph, it ranks the next 5 highest yield transform invocations by expected information gain, with a Spanish/Portuguese native UI for LATAM channel partners.

![Pivotwise working dashboard](outputs/project_working.svg)

## Why it exists

Social Links' own Crimewall page headlines "AI powered link analysis and automation." Under the marketing, the actual AI moments inside an investigation today are mostly classifier level (image recognition, sentiment, OCR) - not the agentic layer that decides which of the 1,500 methods to fire next given a partially built graph.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around social, links, and crimewall.
- Company-specific strategy code in `src/pivotwise/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Pivotwise evidence map](outputs/evidence_map.svg)

## Signals it measures

- `social coverage`
- `links risk`
- `crimewall precision`
- `headlines latency`

## Failure modes it plants

- social drift
- links gap
- crimewall misroute
- headlines blindspot

## Run it locally

```bash
uv sync
uv run pivotwise all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
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

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
