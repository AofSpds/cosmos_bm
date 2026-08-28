# CH-03 — AI-ASSISTED SKIP GO ROUTING

## Identity and provenance

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-03`
- Canonical slug: `ai-assisted-skip-go-routing`
- Decision ID prefix: `BM2-AI-D`
- Role: AI-assisted Routing Research / Deterministic Baseline Comparison Channel
- Packet type: AI routing research / deterministic baseline / shadow mode / no live authority
- Charter source: `sources/raw/channel-policy-packets/v1.0/03_CH03_BM2_AI_SKIP_GO_ROUTING_PACKET.md`
- Charter source SHA-256: `8b38aa15d914f0ca95e83a337da027139d000795372f7f5cdcba6ccd25ceb7ef`
- Source baseline: `COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE`
- Supporting baseline: STEP 3–5 `OWNER-REVIEW CANDIDATE`
- Overall classification: `B. SELECTIVE FIT — CANDIDATE`
- Date (KST): `2026-08-29`

This charter derives from the exact standalone packet above. The raw packet preserves authoritative wording. Bounded AI is `SELECT-LIMITED — CANDIDATE`; current route diversity and Smart-Swap split routing remain existing/assess baselines, not new AI or 6G inventions.

## Authority and decision effect

Authority precedence:

1. Owner's latest explicit decision.
2. CH-00 INTEGRATION / OWNER DECISIONS latest integrated decision.
3. Common hard locks in this charter.
4. Local hard locks and channel-sealed decisions.
5. Working notes, hypotheses, and drafts.

Decision lifecycle: `WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`.

- Conclusions are `CANDIDATE` by default and are not project-final before CH-00 integration and required Owner action.
- This channel does not implicitly alter another channel's scope, authority, or object definitions.
- A changed decision requires a new Decision ID and `SUPERSEDES` reference.

## Authorization boundary

```text
OWNER_ACTION_REQUIRED = FALSE for bootstrap/research/design discussion;
TRUE only for Owner selection, common-boundary change, proposal-text
integration, pilot, or implementation approval.
PRODUCTION_AUTHORIZED = FALSE
FULL_V1_2_REWRITE_AUTHORIZED = FALSE
NEW_BM_AUTHORIZED = FALSE
NATIVE_MODULE_DESIGN_AUTHORIZED = FALSE
LIVE_ROUTING_OR_FINANCIAL_EXECUTION_AUTHORIZED = FALSE
COMMERCIAL_SLA_OR_COMPENSATION_AUTHORIZED = FALSE
FORMAL_6G_CONFORMITY_CLAIM_AUTHORIZED = FALSE
```

Next Owner review: when a Shadow evaluation plan or `BM2-AI-06` Promotion/Hold/Kill choice is ready.

## Four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

CH-03 is a bounded research channel supporting BM2. It does not become a fifth BM and BM1 does not depend on its success.

## Common hard locks

- Preserve `Thin Core, Rich Edges`.
- Base IBC remains open; no forced Hub toll is imposed on base IBC.
- The Hub does not hold customer principal.
- Do not add a Hub-owned DEX, lending service, perpetuals venue, stablecoin, market maker, bridge, or proprietary mandatory/exclusive router as the default design.
- ATOM is not a mandatory payment asset.
- Do not store raw KYC, PII, or an institution's sensitive policy text on a public chain.
- Validate contracts, data, and small audited CosmWasm MVPs before any native module.
- A native module may be considered only after a real recurring operational bottleneck is proven and the Owner separately approves it.
- AI does not hold private keys or approve transactions.
- AI does not unilaterally change hard policy, exposure caps, minimum receive, finality, or allowlists.
- AI does not unilaterally decide compensation, disputes, or legal responsibility.
- Do not imply global atomic revert, principal guarantee, insurance, or guaranteed regulatory fitness.
- Preserve multiple-provider competition, open specifications, and switching.
- Do not use `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.
- The current roadmap is a selective prior-art application candidate, not production-architecture approval.

## Status taxonomy

- `CURRENT IMPLEMENTATION`: functionality actually present in Cosmos, IBC, Skip, wallets, indexers, or adjacent systems.
- `EXISTING / PARTIAL`: functionality currently exists in a limited scope.
- `SOURCE-SUPPORTED FACT`: directly supported by the cited primary source.
- `OFFICIAL ROADMAP / CONTRACTUAL ANNOUNCEMENT`: official direction or contract announcement, not equivalent to operation or realized revenue.
- `V1.2 CHANNEL CANDIDATE`: unintegrated channel proposal.
- `SELECT-LIMITED RESEARCH ITEM`: bounded candidate under hard gates.
- `WATCH`: independent research item awaiting evidence.
- `REJECTED BY GOVERNANCE`: excluded by a hard lock or selection result.
- `OWNER DECISION REQUIRED`: specialist channel cannot settle the choice.
- `CH-00 INTEGRATION REQUIRED`: affects shared objects, priorities, or cross-channel interfaces.

## Primary question and mission

Primary question: does AI prediction reproducibly improve realized outcomes over current Skip Go and rule-based deterministic routing?

Mission: do not presume AI adoption. Freeze current Skip Go as the baseline and evaluate prediction, calibration, drift, abstention, fallback, and net value in M2 Shadow Mode.

## Scope

In scope:

- Current Skip Go route API and routing algorithm.
- Candidate-route generation, quote refresh, liquidity, and slippage.
- Current route diversity and Smart-Swap split as the existing baseline.
- Route-time feature and label availability.
- Latency-distribution prediction.
- Realized-output / slippage prediction.
- Failure probability.
- Recovery probability and expected recovery time.
- Provider anomaly / health signal.
- Risk-adjusted candidate scoring.
- Deterministic optimizer interface.
- Confidence, calibration, abstention, drift, and rollback.
- Model-version binding and feature timestamp.
- Shadow evaluation and adversarial testing.
- Added API, compute, and operations cost.

Out of scope:

- Private key, signature, or transaction authorization.
- Live policy mutation.
- Bridge, asset, or provider allowlist changes.
- Relaxation of exposure cap, minimum receive, or finality.
- Final compensation/breach adjudication.
- Multi-path execution state machine.
- Final factual provider eligibility.
- Hub-owned proprietary mandatory router.
- Production inference authorization.

## Local hard locks

- AI is limited to prediction and advisory ranking.
- The deterministic optimizer and hard-policy engine are authoritative.
- Wallet or institution authorization remains explicit.
- If confidence is insufficient, abstain and fall back to the frozen baseline.
- Do not repackage current Skip Go routing as a new 6G feature.
- Do not claim Smart-Swap split routing as a new AI invention.
- Do not use features with future-information leakage.
- Separate provider rank from eligibility.
- Bind model output to model version, feature time, confidence, and abstention.
- Do not claim live-routing improvement without M2 Shadow results.
- Do not promote on average improvement alone; evaluate p95/p99, failure, recovery, and cost.

## Mandatory deterministic comparators

- Current Skip Go / Default Route
- Shortest Path
- Lowest Quoted Cost
- Maximum Quoted Output
- Minimum Hop
- Rule-based Weighted Score

## Allowed model outputs

- Completion-time distribution
- Realized-output / slippage estimate
- Failure probability
- Recovery probability
- Expected recovery duration
- Provider health / anomaly signal
- Risk-adjusted candidate score
- Human-readable explanation draft

## Prohibited model-output effects

- Direct transaction approval
- Private-key use
- Unregistered provider addition
- Hard-policy override
- Exposure increase
- Minimum-receive reduction
- Finality weakening
- Compensation decision
- Silent route mutation after authorization

## Dependencies and interfaces

- Input from CH-02: frozen feature/label definitions, timestamps, provenance, and recovery states.
- Input from CH-04: route-candidate and leg representation; failover/split classification.
- Input from CH-06: factual capability, provider identity, and evidence freshness.
- Input from CH-07: model responsibility, bias, concentration, economic, and claim boundaries.
- Output to CH-04: route-risk estimates are advisory input, never execution authorization.
- Output to CH-05: prediction, confidence, and explanation schema for structured intent.
- Output to CH-00: Promotion, Hold, permanent Shadow, or Kill recommendation.

## Required outputs

- `BM2-AI-01`: CURRENT_SKIP_GO_AND_DETERMINISTIC_BASELINE
- `BM2-AI-02`: FEATURE_LABEL_AND_DATA_READINESS
- `BM2-AI-03`: SHADOW_EVALUATION_PROTOCOL
- `BM2-AI-04`: CALIBRATION_DRIFT_ABSTENTION_MODEL_GOVERNANCE
- `BM2-AI-05`: BASELINE_COMPARISON_AND_NET_VALUE_REPORT
- `BM2-AI-06`: PROMOTION_HOLD_KILL_RECOMMENDATION

## Evaluation requirements

- Pre-freeze the dataset split and route universe.
- Every feature must be available at quote/decision time.
- Compare every applicable mandatory baseline.
- Measure probability calibration, not only ranking accuracy.
- Test stale/missing data, provider outage, chain halt, price movement, and drift.
- Measure abstention and fallback success.
- Include compute/API latency and operating cost.
- Report performance by asset, chain, provider, and market regime.

## Pass, hold, and kill/permanent shadow

Pass when out-of-sample improvement is reproducible, calibration/tail error is within a defined bound, abstention/fallback is safe, net route value remains positive after added cost, and provider-concentration/discrimination risk is controlled.

Hold when labels are sparse, improvement is route-specific, drift/calibration is unstable, or data freshness/source dependence is excessive.

Kill or remain permanently Shadow when there is no material gain over deterministic baselines, safe abstention/fallback is impossible, added API/compute/operations cost exceeds benefit, ranking reinforces uncontrollable provider-monopoly feedback, or live use would require a hard-lock change.

## Claim rule and validation

- M2 permits only `shadow evaluated` at C2.
- A measured bounded PoC may reach C3 within its exact scope.
- Do not use `AI-optimized production routing` before an operating pilot.
- Validate only changed claims, changed objects, and affected interfaces.
- Do not create full re-research, global regression, or repeated validation loops.
- Distinguish fact, proposal, inference, and unverified hypothesis.
- Without evidence, record `UNKNOWN` or `HOLD` rather than infer.
- Bind `PASS` to exact document, schema, data, code, or contract scope.

Current maximum claim ceiling: `C2 — pre-PoC`.

## Required handoff and reporting shape

A specialist-to-CH-00 handoff separates decision, evidence, impact, and unresolved dependencies. Required fields:

```text
FROM_CHANNEL
DECISION_ID
STATUS
QUESTION
RECOMMENDED_DECISION
ALTERNATIVES_CONSIDERED
EVIDENCE
RATIONALE
IMPACTED_CHANNELS
IMPACTED_BM
IMPACTED_TRACK
HARD_LOCK_CHECK
DEPENDENCIES
LEGAL_SAFETY_ECONOMIC_EFFECT
CLAIM_CEILING
OWNER_ACTION_REQUIRED
PROPOSED_INTEGRATION
SUPERSEDES
```

Use Decision IDs as stable cross-channel references; do not send only a narrative summary. CH-00 registers dependencies when another channel is needed.

Channel progress reporting uses:

```text
OVERALL_PROGRESS
CURRENT_WORKSTREAM
CURRENT_QUESTION
CURRENT_BASELINE
MATERIAL_FINDINGS
DECISION_CANDIDATES
ALTERNATIVES
DEPENDENCIES
RISKS
BLOCKERS
OWNER_ACTION_REQUIRED
NEXT_STEP
```

## Current start point

Close `BM2-AI-01` and `BM2-AI-02` before model selection. No live routing, financial execution, production inference, commercial SLA/compensation, native module, fifth BM, full v1.2 rewrite, or formal 6G claim is authorized.
