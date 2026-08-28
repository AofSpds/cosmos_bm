# CH-03 Topic Index and Discussion Protocol

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
CHANNEL = CH-03 — AI-ASSISTED SKIP GO ROUTING
PERSONA = BM_MASTER
STATUS = CANDIDATE / SELECT-LIMITED RESEARCH / NOT CHANNEL-SEALED
DECISION_ID = BM2-AI-D-0002
EFFECTIVE_SCOPE = CH-03 discussion, memory and reporting protocol only
MODEL_SELECTED = FALSE
LIVE_ROUTING_AUTHORIZED = FALSE
```

This file is the durable topic map for CH-03. It does not promote any AI model,
route policy, live pilot, production architecture, commercial SLA or v1.2 text.
Exact Git state, Owner decisions, `CHANNEL.md`, the channel decision ledger and
primary sources outrank this derived index.

## 1. Owner-directed discussion protocol

Every substantive CH-03 answer follows this order:

1. explain the current item in plain language;
2. enter the technical/hardcore treatment;
3. distinguish current implementation, evidence, inference and proposal;
4. tag Owner locks, Owner questions and later decision points;
5. end with a compact cumulative channel index.

The footer must show at least:

```text
CURRENT_TOPIC
TOPIC_STATUS
BM2-AI-01..06 PROGRESS
OWNER_DECISIONS
OWNER_QUESTIONS
DEPENDENCIES
MEMORY_UPDATE_REQUIRED
NEXT_EXACT_TOPIC
```

## 2. Tag dictionary

| Tag | Meaning |
|---|---|
| `[OWNER-LOCK]` | Current explicit Owner/project hard boundary. It is not reopened by channel inference. |
| `[OWNER-DECIDED]` | Exact scope explicitly decided by the Owner and recorded with no wider implication. |
| `[OWNER-QUESTION]` | A question requiring Owner judgment. The item remains open until answered. |
| `[OWNER-DECISION-LATER]` | No answer is required now; a decision becomes necessary only after the listed evidence gate. |
| `[CHANNEL-CANDIDATE]` | A CH-03 recommendation with no project-final effect. |
| `[RESEARCH-OPEN]` | Evidence or analysis is incomplete. |
| `[DEPENDENCY-CH-XX]` | Another channel owns a required object or decision. |
| `[NO-OWNER-ACTION]` | Bounded research may continue without Owner action. |
| `[HOLD]` | Do not promote or proceed past the named gate. |
| `[KILL]` | Stop this optional track without invalidating unrelated work. |

## 3. Deliverable mapping

| Deliverable | Principal topics |
|---|---|
| `BM2-AI-01` Current Skip Go and deterministic baseline | T02–T05 |
| `BM2-AI-02` Feature, label and data readiness | T06–T11 |
| `BM2-AI-03` Shadow evaluation protocol | T12–T17 |
| `BM2-AI-04` Calibration, drift, abstention and governance | T15–T18 |
| `BM2-AI-05` Baseline comparison and net-value report | T19–T22 |
| `BM2-AI-06` Promotion / Hold / Kill recommendation | T23–T24 |

## 4. Detailed topic map

### T01 — Mission, success definition and authority boundary

**Plain meaning:** Decide what problem AI is allowed to help with and what it is
never allowed to control. The channel succeeds even if AI remains permanently in
Shadow, provided the evaluation proves that deterministic routing is the better
choice.

**Hardcore scope:**

- primary hypothesis: calibrated prediction may improve realized route outcomes;
- null hypothesis: no material net gain over deterministic comparators;
- allowed effects: prediction, anomaly detection, advisory ranking and draft explanation;
- prohibited effects: key custody, signing, transaction approval, allowlist mutation,
  exposure increase, minimum-receive reduction, finality weakening, compensation
  adjudication and silent post-authorization route mutation;
- success states: `PROMOTE_BOUNDED`, `PERMANENT_SHADOW`, `HOLD`, or `KILL`;
- claim ceiling: C2 before a measured bounded PoC.

**Tags:** `[OWNER-LOCK] [OWNER-DECIDED] [NO-OWNER-ACTION]`.

### T02 — Current Skip Go functional baseline

**Plain meaning:** Document what Skip Go already does before calling anything new.

**Hardcore scope:**

- route-request inputs and outputs;
- asset origin and denomination unwind;
- direct-path, channel/client and liquidity selection;
- multi-protocol route composition;
- quote refresh, expiry and transaction tracking;
- status, error, pending, abandoned and recovery-relevant states;
- provider/API boundaries and externally delegated functions;
- current implementation versus partial/undocumented behavior.

**Tags:** `[RESEARCH-OPEN] [NO-OWNER-ACTION]`.

### T03 — Route universe and candidate representation

**Plain meaning:** Define exactly which possible routes are being compared and how
each route is represented.

**Hardcore scope:**

- route, leg, protocol, asset representation and provider identifiers;
- source, intermediate and destination chain sequence;
- route-plan hash and candidate-set timestamp;
- swap, bridge, relay and transfer leg typing;
- route feasibility and unsupported-comparator flags;
- candidate-generation coverage and omission analysis;
- distinction between route candidate, quote and authorized plan.

**Tags:** `[CHANNEL-CANDIDATE] [DEPENDENCY-CH-04] [DEPENDENCY-CH-06]`.

### T04 — Mandatory deterministic comparator suite

**Plain meaning:** AI must beat strong non-AI methods, not a weak strawman.

**Hardcore scope:**

- Current Skip Go / Default Route;
- Shortest Path;
- Lowest Quoted Cost;
- Maximum Quoted Output;
- Minimum Hop;
- Rule-based Weighted Score;
- unsupported-comparator treatment;
- tie-breaking, quote-time consistency and reproducibility;
- comparator version binding and frozen configuration.

**Tags:** `[OWNER-DECIDED] [NO-OWNER-ACTION]`.

### T05 — Objective function and multi-objective trade-offs

**Plain meaning:** A route can be cheaper but slower, or faster but riskier. The
comparison must state what “better” means.

**Hardcore scope:**

- realized output, cost, gas, slippage and completion-time distribution;
- failure, recovery and tail-risk penalties;
- deterministic eligibility constraints versus optimization preferences;
- Pareto frontier before Owner/service-tier weights;
- risk-adjusted utility and regret definitions;
- sensitivity analysis for weight changes;
- service-class-specific objective profiles.

**Tags:** `[RESEARCH-OPEN] [OWNER-DECISION-LATER]`.

### T06 — Evidence and provenance model

**Plain meaning:** Every prediction and outcome must be traceable to where the data
came from.

**Hardcore scope:**

- request/quote, source-chain, per-leg, destination and recovery evidence;
- source transaction, acknowledgement/proof and destination-state corroboration;
- provider feed versus independent indexer distinction;
- evidence source, version, signature/hash, freshness and confidence;
- missing evidence reason codes;
- self-reported evidence limits for financial breach or provider scoring.

**Tags:** `[DEPENDENCY-CH-02] [DEPENDENCY-CH-06] [RESEARCH-OPEN]`.

### T07 — Time, finality and event-order semantics

**Plain meaning:** “How long did it take?” is meaningless unless start, end and
finality are defined consistently.

**Hardcore scope:**

- request, quote, submission, inclusion, acknowledgement and destination-finality time;
- chain-specific finality profiles;
- wall-clock source and clock-skew handling;
- event confidence and delayed/indexer-observed timestamps;
- censoring for unfinished routes;
- quote expiry and stale-feature cutoffs;
- provider-controlled versus external delay windows.

**Tags:** `[DEPENDENCY-CH-02] [RESEARCH-OPEN]`.

### T08 — Feature dictionary

**Plain meaning:** List what the model is allowed to know at decision time.

**Hardcore scope:**

- route topology, hop/leg count and protocol type;
- liquidity, quoted output, fee, gas and slippage indicators;
- client/channel, chain, relayer, bridge and provider health features;
- market volatility and congestion features available at quote time;
- historical provider performance with freshness and confidence;
- missingness indicators and source disagreement;
- prohibited future information and private/sensitive fields.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-02] [DEPENDENCY-CH-06]`.

### T09 — Label and outcome taxonomy

**Plain meaning:** Define what counts as success, failure and recovery before
training anything.

**Hardcore scope:**

- completion and realized-output labels;
- latency distribution and censoring;
- failure cause and controllability;
- recovery probability, location, duration and cost;
- preserved recovery states: `COMPLETED`, `REFUNDED_TO_SOURCE`,
  `RECOVERED_AT_SWAP_CHAIN`, `RECOVERED_AT_INTERMEDIATE`,
  `COMPENSATION_PENDING`, `MANUAL_RECOVERY_REQUIRED`,
  `EXEMPT_EXTERNAL_EVENT`, `UNRESOLVED`;
- provider-health incident labels;
- label delay, revision, uncertainty and adjudication source.

**Tags:** `[DEPENDENCY-CH-02] [DEPENDENCY-CH-04] [DEPENDENCY-CH-07] [RESEARCH-OPEN]`.

### T10 — Data readiness, quality and leakage control

**Plain meaning:** Check whether the data is good enough before choosing a model.

**Hardcore scope:**

- coverage, freshness, completeness and provenance;
- rare-failure and class-imbalance treatment;
- survivorship and success-only sampling bias;
- future-information leakage and label leakage;
- provider, route, asset and regime segmentation;
- source disagreement and independent corroboration;
- reproducibility and licensing/access constraints;
- explicit `READY`, `HOLD` and `NOT_MEASURABLE` outcomes.

**Tags:** `[OWNER-DECIDED] [RESEARCH-OPEN] [NO-OWNER-ACTION]`.

### T11 — Dataset split, route universe freeze and replay set

**Plain meaning:** Freeze the exam before seeing the answers.

**Hardcore scope:**

- chronological train/validation/test split;
- out-of-provider, out-of-route and out-of-regime tests;
- route-universe and inclusion/exclusion criteria;
- incident and tail-event holdout;
- no post-result threshold tuning;
- versioned dataset manifest and feature-time integrity;
- replay dataset limitations and fidelity claims.

**Tags:** `[CHANNEL-CANDIDATE] [OWNER-DECISION-LATER]`.

### T12 — Prediction targets and output contracts

**Plain meaning:** Define exactly what AI may predict and the format of every
prediction.

**Hardcore scope:**

- completion-time distribution;
- realized-output/slippage estimate;
- failure probability;
- recovery probability and expected duration;
- provider-health/anomaly signal;
- risk-adjusted candidate score;
- confidence interval, model version, feature time and abstention field;
- explanation draft separated from the authoritative decision record.

**Tags:** `[OWNER-LOCK] [CHANNEL-CANDIDATE]`.

### T13 — Model hypotheses, not model selection

**Plain meaning:** Compare plausible model families only after the data and task
are fixed. No model is selected now.

**Hardcore scope:**

- transparent statistical and rule-augmented baselines;
- gradient/tree, survival, quantile and probabilistic candidates;
- graph or sequence models only if route representation justifies them;
- ensemble value versus latency/operations cost;
- per-target versus multi-task hypotheses;
- model-capacity, interpretability and deployment-complexity trade-offs;
- ablation plan and model-free null result.

**Tags:** `[OWNER-DECIDED] [RESEARCH-OPEN] [HOLD]` until BM2-AI-01 and BM2-AI-02 close.

### T14 — Deterministic optimizer and hard-policy interface

**Plain meaning:** AI supplies estimates; deterministic code applies rules and
chooses among eligible candidates.

**Hardcore scope:**

- prediction schema consumed by optimizer;
- deterministic eligibility before ranking;
- allowlist, exposure, minimum receive and finality constraints;
- stale/absent prediction behavior;
- published tie-breaking and audit trace;
- model rank separated from factual provider eligibility;
- explicit wallet/institution authorization after disclosure.

**Tags:** `[OWNER-LOCK] [DEPENDENCY-CH-05] [DEPENDENCY-CH-06]`.

### T15 — Calibration and uncertainty

**Plain meaning:** A 10% failure prediction should fail about 10% of the time.

**Hardcore scope:**

- reliability curves and expected calibration error;
- Brier/log score and calibration by segment;
- latency quantile coverage and tail error;
- confidence intervals and prediction sets;
- low-support and out-of-distribution flags;
- calibration decay and recalibration governance;
- calibration thresholds frozen before promotion analysis.

**Tags:** `[RESEARCH-OPEN] [OWNER-DECISION-LATER]`.

### T16 — Abstention and deterministic fallback

**Plain meaning:** When uncertain, the AI must say “I do not know” and return
control to the frozen baseline.

**Hardcore scope:**

- abstention trigger and coverage-risk curve;
- missing/stale feature and source-disagreement triggers;
- out-of-distribution and drift-triggered abstention;
- fallback route identity and version;
- fallback-success and fallback-regret measurement;
- no silent degraded mode;
- manual pause and incident escalation interfaces.

**Tags:** `[OWNER-LOCK] [CHANNEL-CANDIDATE] [OWNER-DECISION-LATER]`.

### T17 — Shadow evaluation protocol

**Plain meaning:** Let AI make recommendations without affecting real transfers,
then compare what would have happened.

**Hardcore scope:**

- pre-registered metrics, thresholds and route universe;
- every applicable comparator;
- realized output, latency, failure, recovery and regret;
- p50/p95/p99 and subgroup reporting;
- counterfactual limitations and selection bias;
- shadow API latency and operational reliability;
- exact code/data/model/version binding;
- no live actuation or production claim.

**Tags:** `[OWNER-DECIDED] [NO-OWNER-ACTION]` for protocol design; promotion requires later Owner action.

### T18 — Drift, robustness and adversarial testing

**Plain meaning:** Test what happens when the market, chains or providers change,
or when data is bad or manipulated.

**Hardcore scope:**

- feature, label and performance drift;
- provider outage, chain halt and congestion shocks;
- stale liquidity/quote and sharp price movement;
- missing/corrupted telemetry and source disagreement;
- provider gaming and strategic reporting;
- anomaly false positives/negatives;
- rollback, quarantine and release governance;
- adversarial scenarios bounded to Shadow/replay first.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-07]`.

### T19 — Provider health, rank, neutrality and concentration

**Plain meaning:** A good model must not turn the largest provider into an
unavoidable monopoly.

**Hardcore scope:**

- factual eligibility versus predictive rank;
- confidence-adjusted provider score;
- self-report dependence and evidence freshness;
- top-provider share and concentration trends;
- newcomer exploration and cold-start treatment;
- switching friction and quote comparability;
- discrimination and feedback-loop audit;
- open schema and no proprietary mandatory Hub router.

**Tags:** `[OWNER-LOCK] [DEPENDENCY-CH-06] [DEPENDENCY-CH-07] [OWNER-DECISION-LATER]`.

### T20 — Provider conflict detection and deterministic arbitration

**Plain meaning:** When providers or models disagree, resolve the conflict by a
published rule rather than a hidden super-agent.

**Hardcore scope:**

- conflicting signed quotes or capability claims;
- stale/incompatible asset representations;
- policy and intent conflicts;
- model disagreement beyond confidence threshold;
- deterministic priorities, rejection reasons and audit trail;
- no model mutation of eligibility;
- escalation to manual review where rules cannot resolve.

**Tags:** `[CHANNEL-CANDIDATE] [DEPENDENCY-CH-05] [DEPENDENCY-CH-06] [DEPENDENCY-CH-07]`.

### T21 — Existing route diversity and Smart-Swap split routing

**Plain meaning:** Treat these as existing/partial capabilities and measure them,
not as new AI inventions.

**Hardcore scope:**

- candidate diversity coverage and trust-path differences;
- split allocation, per-leg result and partial completion;
- extra fee/gas, liquidity impact and recovery surface;
- aggregate completion and accounting;
- current implementation versus proposed broader extension;
- comparator role and no novelty overclaim.

**Tags:** `[OWNER-DECIDED] [EXISTING-ASSESS] [DEPENDENCY-CH-04]`.

### T22 — Sequential failover boundary

**Plain meaning:** Start by replacing an unhealthy route before execution; do not
jump directly to arbitrary mid-flight rerouting.

**Hardcore scope:**

- pre-execution provider/client/channel health check;
- new quote and disclosure after route replacement;
- authorization boundary and route-plan hash;
- unique execution ID, idempotency and duplicate suppression;
- last-known asset location and expired commitment handling;
- post-authorization retry only where provably safe;
- mid-flight mechanisms remain separate and unproven.

**Tags:** `[OWNER-DECIDED] [DEPENDENCY-CH-04] [OWNER-DECISION-LATER]`.

### T23 — Net route value and operating economics

**Plain meaning:** Better predictions are useless if API, compute, support and
recovery costs exceed the benefit.

**Hardcore scope:**

- incremental output/success/tail-latency benefit;
- added provider fee, gas and price impact;
- inference/API latency and direct compute cost;
- monitoring, incident, support and model-governance cost;
- recovery and locked-capital cost;
- concentration/exploration cost;
- segment-specific net value and willingness-to-pay link;
- average-only improvement prohibited.

**Tags:** `[RESEARCH-OPEN] [DEPENDENCY-CH-07] [OWNER-DECISION-LATER]`.

### T24 — Promotion, permanent Shadow, Hold or Kill; claims and integration

**Plain meaning:** At the end, decide whether AI advances, stays advisory forever,
pauses for better data, or is stopped.

**Hardcore scope:**

- reproducible out-of-sample comparator improvement;
- calibration and p95/p99 tail bounds;
- safe abstention/fallback;
- positive net value after all added cost;
- provider-neutrality and concentration controls;
- model/version/evidence auditability;
- claim ladder C0–C4 and C2 current maximum;
- CH-00 handoff with exact evidence and dependencies;
- no automatic v1.2 rewrite, live pilot or production promotion.

**Tags:** `[OWNER-QUESTION] [OWNER-DECISION-LATER] [DEPENDENCY-CH-00]`.

## 5. Owner questions and decision schedule

No immediate answer is required to continue BM2-AI-01 and BM2-AI-02. These
questions become active only at the listed gate.

| ID | Owner question | Activation point | Current state |
|---|---|---|---|
| `BM2-AI-OQ-01` | Which service-objective trade-off should be preferred: output, cost, latency, failure risk or recovery? | after T04 comparator freeze and T05 Pareto analysis | DEFERRED |
| `BM2-AI-OQ-02` | Which assets, chains, protocols and providers define the bounded Shadow route universe? | after T06–T10 data inventory | DEFERRED |
| `BM2-AI-OQ-03` | What minimum evidence/label coverage is acceptable to enter M2 Shadow? | with BM2-AI-02 readiness report | DEFERRED |
| `BM2-AI-OQ-04` | What calibration and p95/p99 tail-risk thresholds are acceptable? | before BM2-AI-03 protocol freeze | DEFERRED |
| `BM2-AI-OQ-05` | How conservative must abstention be, and which frozen fallback is authoritative? | before BM2-AI-03/04 freeze | DEFERRED |
| `BM2-AI-OQ-06` | What concentration limit and newcomer-exploration policy are acceptable? | before any provider-weighting promotion | DEFERRED |
| `BM2-AI-OQ-07` | What added latency/cost and minimum positive net-value hurdle are acceptable? | before BM2-AI-05 conclusion | DEFERRED |
| `BM2-AI-OQ-08` | Promote bounded advisory use, keep permanent Shadow, Hold, or Kill? | BM2-AI-06 | DEFERRED |
| `BM2-AI-OQ-09` | What exact public claim and document placement is approved? | CH-00 integration / revision-scope decision | DEFERRED |

## 6. Current Owner-decided operating points

- `BM2-AI-D-0001`: deterministic baseline and data readiness before model choice;
  M2 Shadow/advisory only; calibrated confidence, abstention and frozen fallback;
  deterministic policy and explicit authorization remain authoritative.
- `BM2-AI-D-0002`: use this detailed topic taxonomy; explain each selected item
  plain-first then hardcore; tag Owner questions and decisions; append the compact
  cumulative channel index to every substantive response; preserve material
  discussion state in channel memory.

Neither decision selects a model, authorizes live routing, seals the channel,
approves a commercial SLA or promotes a v1.2 revision.

## 7. Compact footer template

```text
[CH-03 CUMULATIVE INDEX]
CURRENT_TOPIC = Txx — ...
TOPIC_STATUS = NOT_STARTED / ACTIVE / DRAFTED / FROZEN_CANDIDATE / HOLD / KILL
DELIVERABLE_PROGRESS = AI-01 ... | AI-02 ... | AI-03 ... | AI-04 ... | AI-05 ... | AI-06 ...
OWNER_DECISIONS = D-0001 ... ; D-0002 ...
OWNER_QUESTIONS = OQ-xx DEFERRED/OPEN/ANSWERED
DEPENDENCIES = CH-02 ... ; CH-04 ... ; CH-06 ... ; CH-07 ... ; CH-00 ...
MEMORY_UPDATE_REQUIRED = TRUE/FALSE
NEXT_EXACT_TOPIC = ...
```
