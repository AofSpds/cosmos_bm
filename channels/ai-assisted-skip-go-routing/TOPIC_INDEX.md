# CH-03 Topic Index and Discussion Protocol

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
CHANNEL = CH-03 — AI-ASSISTED SKIP GO ROUTING
PERSONA = BM_MASTER
STATUS = CANDIDATE / SELECT-LIMITED RESEARCH / NOT CHANNEL-SEALED
OWNER_PROTOCOL_DECISION = BM2-AI-D-0002
MODEL_SELECTED = FALSE
LIVE_ROUTING_AUTHORIZED = FALSE
```

This is the durable CH-03 topic map. It does not promote a model, route policy,
live pilot, production architecture, commercial SLA or v1.2 text. Exact Git
state, Owner decisions, `CHANNEL.md`, `DECISIONS.jsonl` and primary sources
outrank this derived index.

## 1. Mandatory discussion protocol

Every substantive CH-03 answer must:

1. explain the selected topic in plain language;
2. continue with the technical/hardcore treatment;
3. distinguish current implementation, evidence, inference and proposal;
4. tag Owner locks, explicit decisions, deferred questions and dependencies;
5. append the compact cumulative CH-03 index at the response bottom.

Material discussion is reflected in `MEMORY.md`, append-only `WORKLOG.md`,
`DECISIONS.jsonl` where applicable, `OPEN_QUESTIONS.md`, and regenerated
`HANDOFF_CURRENT.md`.

## 2. Tag dictionary

| Tag | Meaning |
|---|---|
| `[OWNER-LOCK]` | Current explicit Owner/project boundary; channel inference cannot reopen it. |
| `[OWNER-DECIDED]` | Exact scope explicitly decided by the Owner; no wider implication. |
| `[OWNER-QUESTION]` | Owner judgment is required when the stated activation point is reached. |
| `[OWNER-DECISION-LATER]` | No answer is required now; evidence must be prepared first. |
| `[CHANNEL-CANDIDATE]` | CH-03 recommendation; not project-final. |
| `[RESEARCH-OPEN]` | Evidence or analysis remains incomplete. |
| `[DEPENDENCY-CH-XX]` | Another channel owns a required object or boundary. |
| `[NO-OWNER-ACTION]` | Bounded research can continue without Owner action. |
| `[HOLD]` | Do not proceed past the named gate. |
| `[KILL]` | Stop this optional track without invalidating unrelated work. |

## 3. Deliverable mapping

| Deliverable | Principal topics |
|---|---|
| `BM2-AI-01` Current Skip Go and deterministic baseline | T02–T05 |
| `BM2-AI-02` Feature, label and data readiness | T06–T11 |
| `BM2-AI-03` Shadow evaluation protocol | T12–T17 |
| `BM2-AI-04` Calibration, drift, abstention and governance | T15–T18 |
| `BM2-AI-05` Baseline comparison and net-value report | T17–T23 |
| `BM2-AI-06` Promotion / Permanent Shadow / Hold / Kill | T24 |

## 4. Detailed topic map

### T01 — Mission, success definition and authority boundary

**Plain:** Determine what AI may assist and what it can never control. The
channel can succeed with `PERMANENT_SHADOW` or `KILL` if evidence shows the
frozen deterministic service is safer or more valuable.

**Hardcore:** Primary/null hypotheses; prediction-only authority; prohibited key,
signing, transaction, allowlist, exposure, minimum-receive, finality and
compensation effects; success states `PROMOTE_BOUNDED`, `PERMANENT_SHADOW`,
`HOLD`, `KILL`; C2 pre-PoC ceiling.

**Tags:** `[OWNER-LOCK] [NO-OWNER-ACTION]`.

### T02 — Current Skip Go functional baseline

**Plain:** Record what Skip Go already does before proposing an AI addition.

**Hardcore:** Route-request I/O; asset-origin/denom unwind; direct path,
client/channel and liquidity selection; multi-protocol composition; quote
refresh/expiry; tracking, error, pending and abandoned states; provider/API
boundaries; documented versus partial behavior.

**Tags:** `[RESEARCH-OPEN] [NO-OWNER-ACTION]`.

### T03 — Route universe and candidate representation

**Plain:** Define which routes are eligible for comparison and how each route is
represented.

**Hardcore:** Route/leg/protocol/provider IDs; source/intermediate/destination
sequence; asset representations; route-plan hash; candidate-set time; leg types;
feasibility; candidate omission; candidate versus quote versus authorized plan.

**Tags:** `[CHANNEL-CANDIDATE] [DEPENDENCY-CH-04] [DEPENDENCY-CH-06]`.

### T04 — Mandatory deterministic comparator suite

**Plain:** AI must beat strong non-AI alternatives, not a weak strawman.

**Hardcore:** Current Skip Go/default; shortest path; lowest quoted cost; maximum
quoted output; minimum hop; rule-based weighted score; unsupported applicability;
ties; same quote-time snapshot; versioned frozen configuration.

**Tags:** `[OWNER-LOCK] [NO-OWNER-ACTION]`.

### T05 — Objective function and multi-objective trade-offs

**Plain:** A route can be cheaper but slower or faster but riskier; “better” must
be defined explicitly.

**Hardcore:** Realized output, fee, gas, slippage, latency distribution, failure,
recovery and tail-risk penalties; eligibility constraints versus preferences;
Pareto frontier; risk-adjusted utility/regret; sensitivity; service-class weights.

**Tags:** `[RESEARCH-OPEN] [OWNER-DECISION-LATER]`.

### T06 — Evidence and provenance model

**Plain:** Every input and outcome must be traceable to its source.

**Hardcore:** Request/quote, source-chain, per-leg, destination and recovery
evidence; tx/ack/proof/destination corroboration; provider feed versus independent
indexer; source/version/hash/signature/freshness/confidence; missing-reason codes;
self-report limits for breach and score decisions.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-02] [DEPENDENCY-CH-06]`.

### T07 — Time, finality and event-order semantics

**Plain:** Completion time is meaningless unless start, end and finality are
consistently defined.

**Hardcore:** Request, quote, submission, inclusion, acknowledgement and
destination-finality times; chain-specific finality profiles; clock source/skew;
indexer delay; unfinished-route censoring; quote expiry; stale-feature cutoff;
provider-controlled versus external-delay windows.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-02]`.

### T08 — Feature dictionary

**Plain:** List only information available when a route decision is made.

**Hardcore:** Topology/hops/legs; liquidity, quote, fee, gas and slippage;
client/channel, chain, relayer, bridge and provider health; quote-time volatility
and congestion; historical performance with freshness/confidence; missingness;
source disagreement; prohibited future/private fields.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-02] [DEPENDENCY-CH-06]`.

### T09 — Label and outcome taxonomy

**Plain:** Define success, failure and recovery before training anything.

**Hardcore:** Completion, realized output, latency/censoring, failure cause and
controllability, recovery probability/location/duration/cost, provider incidents,
label delay/revision/uncertainty and adjudication source. Preserve:
`COMPLETED`, `REFUNDED_TO_SOURCE`, `RECOVERED_AT_SWAP_CHAIN`,
`RECOVERED_AT_INTERMEDIATE`, `COMPENSATION_PENDING`,
`MANUAL_RECOVERY_REQUIRED`, `EXEMPT_EXTERNAL_EVENT`, `UNRESOLVED`.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-02] [DEPENDENCY-CH-04] [DEPENDENCY-CH-07]`.

### T10 — Data readiness, quality and leakage control

**Plain:** Decide whether data is good enough before considering a model.

**Hardcore:** Coverage, freshness, completeness, provenance, rare failures,
class imbalance, survivorship/success bias, future/label leakage, segment
coverage, source disagreement, reproducibility, licensing/access, explicit
`READY`, `HOLD`, `NOT_MEASURABLE` dispositions.

**Tags:** `[OWNER-LOCK] [RESEARCH-OPEN] [NO-OWNER-ACTION]`.

### T11 — Dataset split, route-universe freeze and replay set

**Plain:** Freeze the exam before seeing its answers.

**Hardcore:** Chronological train/validation/test; out-of-provider, route and
regime tests; inclusion/exclusion; incident/tail holdout; no post-result threshold
tuning; dataset manifest; feature-time integrity; replay-fidelity limitations.

**Tags:** `[CHANNEL-CANDIDATE] [OWNER-DECISION-LATER]`.

### T12 — Prediction targets and output contract

**Plain:** Define what AI is allowed to predict and the exact shape of its output.

**Hardcore:** Completion-time distribution; realized-output/slippage; failure and
recovery probabilities; expected recovery duration; provider anomaly/health;
risk-adjusted candidate score; model version, feature time, confidence,
abstention and explanation-draft fields.

**Tags:** `[OWNER-LOCK] [CHANNEL-CANDIDATE]`.

### T13 — Model hypotheses, not model selection

**Plain:** Model families are considered only after the problem and data are
frozen. No model is selected now.

**Hardcore:** Transparent statistical/rule baselines; tree/gradient, survival,
quantile and probabilistic candidates; graph/sequence models only if justified;
ensembles versus latency/ops cost; per-target versus multi-task; ablation; null
result; interpretability/deployment burden.

**Tags:** `[OWNER-LOCK] [RESEARCH-OPEN] [HOLD]` until AI-01/02 close.

### T14 — Deterministic optimizer and hard-policy interface

**Plain:** AI supplies estimates; deterministic code enforces rules and selects
among eligible routes.

**Hardcore:** Prediction schema; eligibility before ranking; allowlist, exposure,
minimum receive and finality constraints; stale/absent prediction behavior;
published ties/rejections/audit; rank separated from eligibility; explicit
wallet/institution authorization.

**Tags:** `[OWNER-LOCK] [DEPENDENCY-CH-05] [DEPENDENCY-CH-06]`.

### T15 — Calibration and uncertainty

**Plain:** A 10% predicted failure rate should correspond to roughly 10% actual
failures.

**Hardcore:** Reliability curves, ECE, Brier/log score, segment calibration,
quantile coverage, p95/p99 tail error, confidence intervals/prediction sets,
low-support/OOD flags, calibration decay and frozen promotion thresholds.

**Tags:** `[RESEARCH-OPEN] [OWNER-DECISION-LATER]`.

### T16 — Abstention and deterministic fallback

**Plain:** When uncertain, AI must decline and return control to a known baseline.

**Hardcore:** Coverage-risk curve; missing/stale/disagreement/OOD/drift triggers;
fallback identity/version; fallback success/regret; no silent degraded mode;
manual pause and incident escalation.

**Tags:** `[OWNER-LOCK] [CHANNEL-CANDIDATE] [OWNER-DECISION-LATER]`.

### T17 — Shadow evaluation protocol

**Plain:** AI makes recommendations without affecting transfers, and its
counterfactual performance is measured.

**Hardcore:** Pre-registered route universe, metrics and thresholds; every
applicable comparator; realized output, latency, failure, recovery and regret;
p50/p95/p99 and subgroup results; counterfactual bias; API latency/reliability;
exact data/code/model binding; no live-actuation claim.

**Tags:** `[OWNER-LOCK] [NO-OWNER-ACTION]` for protocol design.

### T18 — Drift, robustness and adversarial testing

**Plain:** Test changing markets, chain/provider incidents and manipulated or bad
data before trusting predictions.

**Hardcore:** Feature/label/performance drift; provider outage; chain halt;
congestion, stale quotes and price shocks; missing/corrupt telemetry; source
disagreement; provider gaming; anomaly errors; rollback/quarantine/release rules;
Shadow/replay-first adversarial tests.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-07]`.

### T19 — Provider health, rank, neutrality and concentration

**Plain:** Prediction must not turn the largest provider into an unavoidable
monopoly.

**Hardcore:** Eligibility versus rank; confidence-adjusted score; self-report
share; evidence freshness; top-provider concentration; newcomer cold start and
exploration; switching/quote comparability; discrimination and feedback loops;
open schema; no mandatory proprietary Hub router.

**Tags:** `[OWNER-LOCK] [DEPENDENCY-CH-06] [DEPENDENCY-CH-07] [OWNER-DECISION-LATER]`.

### T20 — Provider conflict detection and deterministic arbitration

**Plain:** Provider/model disagreements are resolved by published rules, not a
hidden super-agent.

**Hardcore:** Conflicting signed quotes/capabilities; stale or incompatible asset
representations; policy/intent conflicts; model disagreement beyond confidence;
deterministic priorities/reasons/audit; no eligibility mutation; manual review
for unresolved collisions.

**Tags:** `[CHANNEL-CANDIDATE] [DEPENDENCY-CH-05] [DEPENDENCY-CH-06] [DEPENDENCY-CH-07]`.

### T21 — Existing route diversity and Smart-Swap split routing

**Plain:** Measure these existing/partial capabilities; do not call them new AI
or 6G inventions.

**Hardcore:** Candidate coverage and trust paths; split allocation/per-leg result;
partial completion; fee/gas/liquidity/recovery burden; aggregate completion and
accounting; current implementation versus broader extension; comparator role.

**Tags:** `[OWNER-LOCK] [EXISTING-ASSESS] [DEPENDENCY-CH-04]`.

### T22 — Sequential failover boundary

**Plain:** First replace an unhealthy route before execution; arbitrary mid-flight
rerouting is not the starting point.

**Hardcore:** Pre-execution health check; replacement quote/disclosure; approval
boundary; route-plan hash; unique execution ID; idempotency/duplicate suppression;
last-known asset location; expired commitments; post-authorization retry only
where provable; mid-flight remains unverified.

**Tags:** `[OWNER-LOCK] [DEPENDENCY-CH-04] [OWNER-DECISION-LATER]`.

### T23 — Net route value and operating economics

**Plain:** Intelligence is not valuable when compute, API, support and recovery
costs exceed its benefit.

**Hardcore:** Incremental output/success/tail-latency; provider fee, gas and price
impact; inference/API cost and delay; monitoring, incident, support and governance
cost; recovery and locked capital; exploration/concentration cost; segment net
value; willingness to pay; average-only improvement prohibited.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-07] [OWNER-DECISION-LATER]`.

### T24 — Promotion, Permanent Shadow, Hold or Kill; claims and integration

**Plain:** Decide whether AI advances, remains advisory forever, pauses for better
data, or stops.

**Hardcore:** Reproducible out-of-sample gain; calibration/tail bounds; safe
abstention/fallback; positive net value; neutrality/concentration; model/evidence
auditability; claim ladder C0–C4 with current C2 maximum; CH-00 handoff; no
automatic rewrite, live pilot or production promotion.

**Tags:** `[OWNER-QUESTION] [OWNER-DECISION-LATER] [DEPENDENCY-CH-00]`.

## 5. Deferred Owner questions and activation schedule

No immediate answer is required for `BM2-AI-01` or `BM2-AI-02`.

| ID | Owner question | Activation point | State |
|---|---|---|---|
| `BM2-AI-OQ-01` | Preferred trade-off among output, cost, latency, failure risk and recovery? | after T04/T05 evidence | DEFERRED |
| `BM2-AI-OQ-02` | Which assets, chains, protocols and providers form the bounded Shadow universe? | after T06–T10 inventory | DEFERRED |
| `BM2-AI-OQ-03` | Minimum evidence/label/provenance coverage to enter M2? | with AI-02 report | DEFERRED |
| `BM2-AI-OQ-04` | Acceptable calibration and p95/p99 tail thresholds? | before AI-03 freeze | DEFERRED |
| `BM2-AI-OQ-05` | Abstention strictness and authoritative frozen fallback? | before AI-03/04 freeze | DEFERRED |
| `BM2-AI-OQ-06` | Provider concentration limit and newcomer-exploration policy? | before weighting promotion | DEFERRED |
| `BM2-AI-OQ-07` | Acceptable added latency/cost and minimum positive net-value hurdle? | before AI-05 conclusion | DEFERRED |
| `BM2-AI-OQ-08` | Promote bounded advisory use, Permanent Shadow, Hold or Kill? | AI-06 | DEFERRED |
| `BM2-AI-OQ-09` | Approved public claim and document placement? | CH-00/revision scope | DEFERRED |

## 6. Decision-status readback

- `BM2-AI-D-0001` = `[CHANNEL-CANDIDATE]`: deterministic baseline and data
  readiness before model choice; M2 Shadow/advisory; calibrated confidence,
  abstention and frozen fallback; deterministic policy and explicit
  authorization remain authoritative.
- `BM2-AI-D-0002` = `[OWNER-DECIDED]`: use this durable taxonomy; explain each
  topic plain-first then technically; tag Owner decisions/questions; append the
  cumulative footer; persist material discussion state.

Neither record selects a model, authorizes live routing, seals the channel,
approves a commercial SLA or promotes a v1.2 revision.

## 7. Compact footer template

```text
[CH-03 CUMULATIVE INDEX]
CURRENT_TOPIC = Txx — ...
TOPIC_STATUS = NOT_STARTED / ACTIVE / DRAFTED / FROZEN_CANDIDATE / HOLD / KILL
DELIVERABLE_PROGRESS = AI-01 ... | AI-02 ... | AI-03 ... | AI-04 ... | AI-05 ... | AI-06 ...
OWNER_DECISIONS = D-0001 CANDIDATE ; D-0002 OWNER_DECIDED
OWNER_QUESTIONS = OQ-xx DEFERRED / OPEN / ANSWERED
DEPENDENCIES = CH-02 ... ; CH-04 ... ; CH-05 ... ; CH-06 ... ; CH-07 ... ; CH-00 ...
MEMORY_UPDATE_REQUIRED = TRUE / FALSE
NEXT_EXACT_TOPIC = ...
```
