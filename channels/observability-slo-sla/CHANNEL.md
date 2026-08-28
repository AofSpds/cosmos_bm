# CH-02 — OBSERVABILITY / SLO / SLA

## Identity and provenance

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-02`
- Canonical slug: `observability-slo-sla`
- Decision ID prefix: `BM2-EVID-D`
- Role: BM2 Evidence Foundation / Observability / SLO / SLA Semantics Channel
- Packet type: evidence foundation / time semantics / failure-recovery taxonomy / SLO-SLA model / no commercial guarantee
- Charter source: `sources/raw/channel-policy-packets/v1.0/02_CH02_BM2_OBSERVABILITY_SLO_SLA_PACKET.md`
- Charter source SHA-256: `4263407306475bf124a5da4e61c1d692662dcf02e64827ab725c1ce9af543ec8`
- Source baseline: `COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE`
- Supporting baseline: STEP 3–5 `OWNER-REVIEW CANDIDATE`
- Overall classification: `B. SELECTIVE FIT — CANDIDATE`
- Date (KST): `2026-08-29`

This charter derives from the exact standalone packet above. The raw packet preserves authoritative wording. `SELECT` in the STEP 3–5 portfolio is still a Candidate recommendation, not an Owner decision or a commercial SLA authorization.

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

Next Owner review: when `BM2-EVID-01` through `BM2-EVID-06` Candidates close and a choice on the M1 Data Gate or M3 SLA scope is required.

## Four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

CH-02 owns the shared evidence foundation for BM2 and interfaces to the other BMs; it does not change the order or create a fifth BM.

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

Primary question: how can completion, failure, and recovery of an Interchain transaction be measured objectively, and which of those measurements can support an SLO or bounded commercial SLA?

Mission: establish provenance-aware evidence, time semantics, failure/recovery taxonomy, and deterministic measurement authority before AI, failover, or commercial compensation.

## Scope

In scope:

- Request, Quote, Execution, Leg, Destination, and Recovery evidence.
- Quote, Inclusion, Finality, Relay, Swap, Bridge, Completion, Recovery, and Compensation time.
- Source-chain and destination-chain finality criteria.
- Reconciliation among provider telemetry, chain evidence, and independent indexers.
- Missing, stale, and conflicting-source handling.
- Failure causes and provider controllability.
- Last-known asset location.
- Recovery State and evidence completeness.
- Separation among Metric, SLO, Commercial SLA, Compensation, and Insurance.
- Measurable conditions in a Signed Quote.
- Breach, exempt external event, and unresolved state.
- Receipt schema and dispute evidence.
- Common evidence interface for BM1 attribution, BM3 reporting, and BM4 history.

Out of scope:

- AI model architecture and provider ranking.
- Live route failover execution.
- Final commercial bond size, reserve, or insurance law.
- Institution policy UX/API.
- Provider-eligibility business policy.
- Naming one indexer as sole adjudicator.
- Global finality, atomicity, or principal guarantee.

## Local hard locks

- Maintain `Metric ≠ SLO ≠ Commercial SLA ≠ Compensation ≠ Insurance`.
- Distinguish `destination tx observed` from `agreed finality reached`.
- Do not use one provider API status as final legal truth.
- Do not use a single indexer as sole breach authority.
- Lower confidence when provider self-report lacks independent evidence.
- State timestamp source, clock semantics, and freshness.
- Do not treat missing evidence as success.
- Separate chain halt, bridge halt, user error, and provider-controlled failure.
- Do not imply global atomic revert or guaranteed delivery.
- Do not include raw PII or institution-sensitive information in public evidence.

## Preserved recovery states

- `COMPLETED`
- `REFUNDED_TO_SOURCE`
- `RECOVERED_AT_SWAP_CHAIN`
- `RECOVERED_AT_INTERMEDIATE`
- `COMPENSATION_PENDING`
- `MANUAL_RECOVERY_REQUIRED`
- `EXEMPT_EXTERNAL_EVENT`
- `UNRESOLVED`

These labels are state/taxonomy Candidates; they do not authorize compensation or guarantee recovery.

## Minimum time model

- Quote Time and Quote Expiry
- Authorization Time
- Source Inclusion Time and Source Finality Time
- Leg Start / End Time
- Relay Time, Swap Time, Bridge Time
- Destination Inclusion Time and Destination Finality Time
- Total Completion Time
- Failure Detection Time
- Recovery Start / End Time
- Compensation Decision / Payout Time

## Evidence hierarchy

1. Source transaction/state and cryptographic protocol evidence.
2. Destination transaction/state.
3. Packet acknowledgement, timeout, or bridge-specific state.
4. Independent indexer reconciliation.
5. Provider-signed telemetry.
6. Operator narrative or manual incident note.

When only lower-tier evidence exists, record that fact and do not overstate confidence.

## Dependencies and interfaces

- Input from CH-01: Campaign attribution events and revenue-evidence requirements.
- Input from CH-03: feature/label needs and leakage-prevention constraints.
- Input from CH-04: route leg, failover point, split/aggregate completion, and recovery invariant.
- Input from CH-05: institutional-report and service-class SLO requirements.
- Input from CH-06: provider capability/history and evidence-freshness reference.
- Input from CH-07: breach, exempt event, compensation, and legal-responsibility boundary.
- Output to all: canonical telemetry, time, failure, recovery, SLO, and evidence semantics.

## Required outputs

- `BM2-EVID-01`: TELEMETRY_AND_PROVENANCE_SCHEMA
- `BM2-EVID-02`: TIME_AND_FINALITY_SEMANTICS
- `BM2-EVID-03`: FAILURE_RECOVERY_CONTROLLABILITY_TAXONOMY
- `BM2-EVID-04`: INTERCHAIN_SLO_DICTIONARY
- `BM2-EVID-05`: SLA_BREACH_EXCEPTION_EVIDENCE_RULE
- `BM2-EVID-06`: INDEPENDENT_RECONCILIATION_AND_DISPUTE_PROTOCOL

## Decision questions

- Which event proves completion?
- How is finality defined per chain profile?
- How are provider-controllable breach and external event separated?
- When can last-known asset location be established?
- Which missingness makes an SLA determination `HOLD`?
- What is the boundary between minimum on-chain receipt and detailed off-chain evidence?
- Which metrics alone are contractible in a bounded M3 pilot?

## Pass, hold, and kill/scope reduction

Pass when a pilot-scope route's completion/recovery is reproducible, timestamp/finality/provenance is explicit, provider self-report can be reconciled with independent evidence, SLO/breach is objectively determinable, and last-known asset location is recoverable in failure simulation.

Hold when failure/recovery labels are insufficient, source disagreement lacks a resolution rule, finality/time semantics are unclear, or evidence visibility conflicts with the privacy boundary.

Kill/reduce scope when the service is not objectively measurable, recovery state cannot be reconstructed, commercial rights depend on one provider's discretionary status, or SLA exposure outruns evidence quality.

## Validation and claim ceiling

- Validate only changed claims, changed objects, and affected interfaces.
- Do not create full re-research, global regression, or repeated validation loops.
- Distinguish fact, proposal, inference, and unverified hypothesis.
- Without evidence, record `UNKNOWN` or `HOLD` rather than fill a gap by inference.
- Bind `PASS` to the exact document, schema, data, code, or contract scope.
- A failure in one optional track does not invalidate unrelated tracks.

Claim ladder: C0 internal hypothesis; C1 structural alignment; C2 selective design referencing official research; C3 measured bounded PoC; C4 scope-disclosed operating pilot; C5 only after formal conformity assessment. Current maximum: `C2 — pre-PoC`.

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

Freeze `BM2-EVID-01` through `BM2-EVID-03` before AI or SLA pricing. STEP 3–5 marks Observability/Evidence and the Interchain SLO/SLA Evidence Model `SELECT — CANDIDATE`; no commercial SLA, live routing, or production authority follows.
