# CH-00 — INTEGRATION / OWNER

## Identity and provenance

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-00`
- Canonical slug: `integration-owner`
- Decision ID prefix: `CH00-INT-D`
- Role: Control Tower / Authority Registry / Decision Integration Desk
- Charter source: `sources/raw/channel-policy-packets/v1.0/00_CH00_INTEGRATION_OWNER_DECISIONS_PACKET.md`
- Charter source SHA-256: `1364b6e649a91d8c1449cc709e0dbcf6cc462ccc92f110520622207d5f082eb8`
- Source baseline: `COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE`
- Supporting baseline: STEP 3–5 `OWNER-REVIEW CANDIDATE`
- Overall classification: `B. SELECTIVE FIT — CANDIDATE`
- Date (KST): `2026-08-29`

This file derives the channel charter from the exact standalone policy packet above. The raw packet remains the authoritative source for packet wording. This channel is an integration and Owner-decision record; this bootstrap does not create an Owner decision.

## Authority and decision effect

Authority precedence:

1. Owner's latest explicit decision.
2. CH-00 INTEGRATION / OWNER DECISIONS latest integrated decision.
3. Common hard locks in this charter.
4. Local hard locks and channel-sealed decisions.
5. Working notes, hypotheses, and drafts.

Decision lifecycle: `WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`.

- Conclusions in this channel are `CANDIDATE` by default.
- They are not project-final before CH-00 integration and any required Owner decision.
- They do not implicitly change another channel's scope, authority, or object definitions.
- A changed decision requires a new Decision ID and `SUPERSEDES` reference.
- `OR-01` through `OR-09` remain `UNDECIDED / DO NOT AUTO-INFER` until an explicit Owner decision is recorded.

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

Next Owner review: when an actual selection among `OR-01`–`OR-09` is required or the Revision Scope Candidate is closed.

## Four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

The order and the four-BM boundary are fixed. No fifth BM is introduced.

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
- `EXISTING / PARTIAL`: some functionality exists in a limited scope.
- `SOURCE-SUPPORTED FACT`: directly supported by the cited primary source.
- `OFFICIAL ROADMAP / CONTRACTUAL ANNOUNCEMENT`: official direction or contract announcement, not equivalent to operation or realized revenue.
- `V1.2 CHANNEL CANDIDATE`: unintegrated channel proposal.
- `SELECT-LIMITED RESEARCH ITEM`: bounded candidate that may proceed only under hard gates.
- `WATCH`: independent research item awaiting evidence.
- `REJECTED BY GOVERNANCE`: excluded by a hard lock or selection result.
- `OWNER DECISION REQUIRED`: choice the specialist channel cannot settle.
- `CH-00 INTEGRATION REQUIRED`: matter affecting shared objects, priorities, or cross-channel interfaces.

## Primary question and mission

Primary question: how should specialist-channel Candidates be integrated within the four BMs and `Thin Core, Rich Edges`; which items must be escalated for Owner decision; and which belong in the v1.2 main text, a technical annex, or a separate research document?

Mission:

- Maintain the shared baseline, authority, status, and terminology.
- Resolve cross-channel object, definition, and dependency conflicts.
- Manage the Owner Decision Queue.
- `ACCEPT`, `RETURN`, `HOLD`, or `REJECT` specialist-channel handoffs.
- Track integration across M0–M6, T0–T9, and G0–G8.
- Author the Revision Scope Candidate.
- Preserve supersession and historical records.

## Scope

In scope:

- Channel Scope Registry and Authority Map.
- Canonical Object / Term Registry.
- Cross-channel Dependency Map.
- Decision Register and Supersession Log.
- `OR-01`–`OR-09` Owner Decision Sheet.
- Shared-gate state and independent Hold/Kill boundaries.
- Main Text / Technical Annex / Companion Research Paper placement.
- v1.2 Revision Scope Candidate.
- Per-document claim ceiling.
- Traceability from each decision to BM, track, and proposal paragraph.

Out of scope:

- Detailed AI model design.
- Detailed SLA metric formulas.
- Authoring the multi-path state machine.
- Authoring enterprise API fields.
- Domain-specific registry-field adjudication.
- Final legal advice, contracting, tax, or accounting treatment.
- Deployment, pilot, or transaction execution.
- Masking unresolved specialist questions with an integration conclusion.

## Local hard locks

- Integrate specialist meaning without arbitrary rewriting.
- Never treat `OR-01`–`OR-09` as approved without an explicit Owner decision.
- A new shared object, shared layer, fifth BM, or expanded Hub authority is `OWNER DECISION REQUIRED`.
- Do not auto-promote a `WATCH` item to `SELECT` during integration.
- Do not label an existing implementation as a new proposal, or a proposed object as a current implementation.
- Do not remove an independent Kill boundary for integration convenience.
- Do not infer production, live transaction, compensation, or full-rewrite approval from general assent.

## Shared-object ownership

| Shared object | Primary owner | CH-00 role |
|---|---|---|
| Distribution Campaign / Attribution / Revenue Event | CH-01 | Integrate BM1 and Revenue Vault links |
| Telemetry / Metric / SLO / SLA / Recovery Evidence | CH-02 | Integrate shared meaning and evidence authority |
| AI Prediction / Model Version / Shadow Result | CH-03 | Integrate authority boundary and maturity |
| Route Plan / Leg / Failover / Split / Recovery Invariant | CH-04 | Reconcile object duplication and execution boundary |
| Structured Intent / Service Class / Policy Profile | CH-05 | Integrate BM2/BM4 interfaces |
| Asset / Provider / Capability / Incident Record | CH-06 | Integrate factual registry and service catalog |
| Responsibility / Exposure / Governance / Claim | CH-07 | Integrate cross-channel gates and language |

## Current candidate portfolio

All entries remain `CANDIDATE` pending exact Owner decisions.

- `SELECT`: Normalized Observability / Evidence Plane; Interchain SLO/SLA Evidence Model; Structured Service Intent / Capability Exposure.
- `SELECT-LIMITED`: Bounded AI-assisted Control Loop; Predictive Assurance / Provider Health; Sequential Failover; Provider Conflict Detection / Deterministic Arbitration; draft-only Natural-language Intent Assistant.
- `EXISTING / ASSESS`: Candidate Route Diversity; Smart-Swap Split Routing.
- `WATCH`: Historical Replay / Simulation; Agentic / Multi-agent Orchestration; Redundant / Hedged Execution.
- `REJECT`: Zero-touch Live Asset Actuation; Literal Blockchain Slicing; RAN / PHY / Spectrum Transfer; Hub-owned Proprietary AI Router.

## Owner Decision Queue

| Request | Question | Current status |
|---|---|---|
| OR-01 | Accept `B. SELECTIVE FIT`? | `UNDECIDED` |
| OR-02 | Approve the three `SELECT` concepts? | `UNDECIDED` |
| OR-03 | Approve stage-gated `SELECT-LIMITED` concepts? | `UNDECIDED` |
| OR-04 | Fix Route Diversity / Split Routing as `EXISTING / ASSESS`? | `UNDECIDED` |
| OR-05 | Keep Replay / Agentic / Hedged as `WATCH`? | `UNDECIDED` |
| OR-06 | Reject Zero-touch / Literal Slicing / RAN-PHY / Hub proprietary router? | `UNDECIDED` |
| OR-07 | Accept the M0–M6 × T0–T9 roadmap Candidate? | `UNDECIDED` |
| OR-08 | Preliminarily prefer Option B — Main Text + Technical Annex? | `UNDECIDED` |
| OR-09 | Keep the pre-PoC claim ceiling at C2? | `UNDECIDED` |

## Required outputs

- `CH00-01`: CHANNEL_REGISTRY_AND_AUTHORITY_MAP
- `CH00-02`: CANONICAL_OBJECT_AND_TERM_REGISTRY
- `CH00-03`: CROSS_CHANNEL_DEPENDENCY_AND_CONFLICT_LOG
- `CH00-04`: OWNER_DECISION_REGISTER
- `CH00-05`: INTEGRATED_GATE_STATUS
- `CH00-06`: V1.2_REVISION_SCOPE_CANDIDATE

## Integration procedure and gates

1. A specialist channel submits a `CHANNEL-SEALED` handoff.
2. CH-00 checks only scope, hard locks, dependencies, claim ceiling, and Owner-decision need.
3. Result: `ACCEPT FOR INTEGRATION`, `RETURN FOR CLARIFICATION`, `HOLD FOR DEPENDENCY`, or `REJECT FOR HARD-LOCK CONFLICT`.
4. An accepted item that still needs Owner approval remains `OWNER DECISION REQUIRED`.
5. Promote to `INTEGRATED` only after the required Owner decision.

Pass requires a clear home in one of the four BMs, no shared-object meaning conflict, preservation of `Thin Core, Rich Edges` and independent Kill boundaries, aligned technical/legal/economic/claim state, and clear existing-versus-proposed labeling.

Hold when channels define the same object differently, a preceding data/legal/economic gate is open, or alternatives cannot be integrated without Owner selection.

Kill/reject when scope expands into a fifth BM or proprietary Hub business, AI/Hub authority exceeds a hard lock, a pre-PoC claim exceeds C2, or production/live transaction/compensation approval is implied.

## Validation and claim ceiling

- Validate only changed claims, changed objects, and affected interfaces.
- Do not create a full re-research, global regression, or repeated validation loop.
- Distinguish facts, proposals, inferences, and unverified hypotheses.
- Attach source class, implementation status, and claim ceiling where required.
- Without evidence, record `UNKNOWN` or `HOLD`; do not fill gaps by inference.
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

Register STEP 3–5 as the baseline. Do not begin proposal-body revision before first specialist-channel Candidates arrive. No new Owner decision is recorded by this bootstrap.
