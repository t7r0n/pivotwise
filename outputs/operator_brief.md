# Operator Brief: Social Links

Social Links gets a local, deterministic pressure test around social, links, and crimewall. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- social evidence replay -> block release until cited evidence is regenerated (social_coverage, evidence ev_0044).
- headlines operator packet -> accept only if decision claims cite fixture evidence (links_risk, evidence ev_0011).
- crimewall regression harness -> open a regression issue with trace and benchmark delta (crimewall_precision, evidence ev_0110).
- links boundary probe -> route to reviewer with evidence packet (headlines_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
