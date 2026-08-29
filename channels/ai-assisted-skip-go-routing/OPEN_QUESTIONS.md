# CH-03 Open Questions

All questions remain bounded CH-03 research questions unless marked
`[OWNER-QUESTION]`. No live-routing authority, production claim, model choice or
channel seal is inferred. Detailed topic ownership appears in `TOPIC_INDEX.md`.

## A. Baseline and data readiness — research may proceed now

- `[PARTIAL-CLOSURE][T02]` Current official documentation establishes the broad
  Skip Go product flow, the narrow IBC origin/unwind/direct-liquidity algorithm,
  route/quote and operation fields, transaction-message construction,
  user-signer execution integration, tracking/status and protocol-specific
  failure behavior. T02 is not frozen because the questions below remain open.
- `[RESEARCH-OPEN][T02]` Is there a public versioned route-engine or registry
  release identifier that can be bound to every observation?
- `[RESEARCH-OPEN][T02]` Which route defaults vary by endpoint, client version,
  API-key/access tier or server-side configuration?
- `[RESEARCH-OPEN][T02/T03]` Can Skip Go expose the complete candidate set and
  rejected candidates, or only the selected route and operations?
- `[RESEARCH-OPEN][T02/T06-T10]` What historical route, quote, status, failure,
  recovery and feature-time data are accessible under reproducible terms?
- `[RESEARCH-OPEN][T02/T17]` Which Smart Relay capabilities and relay mode were
  active for each historical route observation?
- `[RESEARCH-OPEN][T02/T06]` Which `/status` fields can be independently
  corroborated from chain, packet, bridge and indexer evidence?
- `[CHANNEL-CANDIDATE][T02/T04]` Should the comparator retain both
  `B0-A SKIP_DEFAULT_AS_SERVED` and `B0-B SKIP_EXPLICIT_FROZEN_CONFIG`?
- `[RESEARCH-OPEN][T03]` What exact route/leg/candidate representation is needed
  for reproducible comparison?
- `[RESEARCH-OPEN][T04]` Which of the six mandatory deterministic comparators
  apply to each route universe, and how is unsupported applicability recorded?
- `[RESEARCH-OPEN][T06-T08]` Which features are actually available at
  quote/decision time, with timestamp, provenance, confidence and freshness?
- `[RESEARCH-OPEN][T09]` Which completion, realized-output/slippage, failure,
  recovery and provider-health labels are sufficiently complete and independently
  corroborated?
- `[RESEARCH-OPEN][T10]` How are future-information leakage, stale/missing data,
  source disagreement, rare failures, survivorship and provider self-report bias
  controlled?
- `[RESEARCH-OPEN][T11]` Which route universe, inclusion/exclusion rule and
  chronological dataset split can be frozen before evaluation?

## B. Shadow evaluation and model governance — activated after AI-01/02

- `[RESEARCH-OPEN][T12]` Which model outputs are measurable and operationally
  useful without creating authority over eligibility or execution?
- `[RESEARCH-OPEN][T13]` Which model families merit hypothesis testing after the
  data and tasks are frozen? No model is selected now.
- `[RESEARCH-OPEN][T15]` Which calibration metrics and segment-level reliability
  tests are required?
- `[RESEARCH-OPEN][T16]` Under what objective conditions must the model abstain,
  and how is deterministic fallback verified?
- `[RESEARCH-OPEN][T17]` Which out-of-sample metrics demonstrate material
  improvement over every applicable deterministic baseline?
- `[RESEARCH-OPEN][T18]` Does fallback remain safe during missing data, provider
  outage, chain halt, quote staleness, price movement, source disagreement and
  drift?
- `[RESEARCH-OPEN][T23]` What compute/API latency, operations, monitoring,
  incident, recovery and governance cost must be deducted from net route value?
- `[RESEARCH-OPEN][T17-T23]` How does performance vary by asset, chain, route,
  provider and market regime, including p95/p99 tails?

## C. Provider neutrality and operational boundaries

- `[RESEARCH-OPEN][T19]` How are provider rank and factual eligibility kept
  separate in data, optimizer and user-facing outputs?
- `[RESEARCH-OPEN][T19]` Which confidence, concentration, switching and newcomer
  exploration metrics prevent self-reinforcing provider dominance?
- `[RESEARCH-OPEN][T20]` How are conflicting signed quotes, capability claims,
  provider data and model outputs resolved by public deterministic rules?
- `[RESEARCH-OPEN][T21]` What incremental net value and recovery burden arise
  from existing route diversity and Smart-Swap split routing?
- `[RESEARCH-OPEN][T22]` Which exact pre-execution failover point, quote refresh,
  authorization boundary, unique ID and idempotency rules are safe?

## D. Deferred Owner questions

No immediate Owner answer is required for `BM2-AI-01` or `BM2-AI-02`. Each
question activates only after the prerequisite evidence is prepared.

| ID | Tag | Question | Activation point | State |
|---|---|---|---|---|
| `BM2-AI-OQ-01` | `[OWNER-QUESTION][T05]` | Which service-objective trade-off should be preferred among realized output, total cost, latency, failure risk and recovery? | after comparator freeze and Pareto analysis | DEFERRED |
| `BM2-AI-OQ-02` | `[OWNER-QUESTION][T03/T11]` | Which assets, chains, protocols and providers define the bounded Shadow route universe? | after data inventory | DEFERRED |
| `BM2-AI-OQ-03` | `[OWNER-QUESTION][T10]` | What minimum evidence, label and provenance coverage is acceptable to enter M2 Shadow? | with `BM2-AI-02` | DEFERRED |
| `BM2-AI-OQ-04` | `[OWNER-QUESTION][T15/T17]` | What calibration and p95/p99 tail-risk thresholds are acceptable? | before `BM2-AI-03` freeze | DEFERRED |
| `BM2-AI-OQ-05` | `[OWNER-QUESTION][T16]` | How conservative must abstention be, and which frozen deterministic fallback is authoritative? | before `BM2-AI-03/04` freeze | DEFERRED |
| `BM2-AI-OQ-06` | `[OWNER-QUESTION][T19]` | What provider concentration limit and newcomer-exploration policy are acceptable? | before provider weighting promotion | DEFERRED |
| `BM2-AI-OQ-07` | `[OWNER-QUESTION][T23]` | What added latency/cost and minimum positive net-value hurdle are acceptable? | before `BM2-AI-05` conclusion | DEFERRED |
| `BM2-AI-OQ-08` | `[OWNER-QUESTION][T24]` | Promote bounded advisory use, keep permanent Shadow, Hold, or Kill? | `BM2-AI-06` | DEFERRED |
| `BM2-AI-OQ-09` | `[OWNER-QUESTION][T24]` | What exact public claim and document placement is approved? | CH-00 integration / revision-scope decision | DEFERRED |

## E. Cross-channel closures required before channel seal

- `[DEPENDENCY-CH-02]` feature/label/time/provenance/recovery semantics;
- `[DEPENDENCY-CH-04]` route/leg/state/failover and asset-location model;
- `[DEPENDENCY-CH-05]` structured-intent, policy and disclosure interface;
- `[DEPENDENCY-CH-06]` factual provider identity/capability/evidence freshness;
- `[DEPENDENCY-CH-07]` responsibility, concentration, discrimination, liability,
  claim and economic limits;
- `[DEPENDENCY-CH-00]` final Promotion/Hold/Kill and v1.2 integration decision.

Owner action becomes mandatory only for an activated Owner question, actual
promotion choice, transaction-affecting pilot, live/production inference,
implementation, proposal-text integration or another separately controlled
approval.
