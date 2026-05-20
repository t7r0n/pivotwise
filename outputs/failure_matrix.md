# Failure Matrix: Pivotwise

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| social evidence replay | social_drift | social_coverage | block release until cited evidence is regenerated | ev_0000 |
| headlines operator packet | headlines_blindspot | headlines_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| headlines operator packet | headlines_blindspot | headlines_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| crimewall regression harness | crimewall_misroute | crimewall_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| links boundary probe | links_gap | links_risk | route to reviewer with evidence packet | ev_0021 |
| crimewall regression harness | crimewall_misroute | crimewall_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| social evidence replay | social_drift | social_coverage | block release until cited evidence is regenerated | ev_0028 |
