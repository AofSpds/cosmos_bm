# CH-03 Open Questions

All questions remain open bounded-research questions. No Owner decision, live-routing authority, or production claim is inferred.

## Baseline and data readiness

- What exact current Skip Go route API/algorithm behavior defines the frozen baseline?
- Which of the six mandatory deterministic comparators apply to each route universe?
- Which features are actually available at quote/decision time, with timestamp, provenance, and freshness?
- Which completion, realized-output/slippage, failure, recovery, and provider-health labels are sufficiently complete?
- How are future-information leakage, stale/missing data, source disagreement, and rare failures controlled?
- Which route universe and dataset split can be pre-registered before evaluation?

## Shadow evaluation

- Which model outputs materially improve outcomes over every applicable baseline out of sample?
- What probability-calibration and p95/p99 tail-error thresholds are acceptable?
- Under what confidence threshold must the model abstain?
- Does frozen-baseline fallback succeed during missing data, provider outage, chain halt, price movement, and drift?
- What compute/API latency and operating cost must be deducted from net route value?
- How does performance vary by asset, chain, provider, and market regime?

## Governance and promotion

- How are provider rank and factual eligibility kept separate?
- Which concentration/discrimination feedback metrics trigger Hold or Kill?
- What exact evidence supports Promotion, permanent Shadow, Hold, or Kill in `BM2-AI-06`?
- Which CH-02, CH-04, CH-06, and CH-07 dependencies must close before the Shadow plan is channel-sealed?

Owner action is not required for bounded baseline/data/shadow design. It becomes required for an actual promotion choice, transaction-affecting pilot, live/production inference, implementation, text integration, or another separately controlled approval.
