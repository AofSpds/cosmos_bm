# CH-01 — DISTRIBUTION MARKET / REVENUE

## Identity and provenance

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-01`
- Canonical slug: `distribution-market-revenue`
- Decision ID prefix: `BM1-DIST-D`
- Role: BM1 Product / Market / Revenue Evidence Design Channel
- Packet type: BM1 product design / attribution / anti-gaming / revenue evidence / no AI dependency
- Charter source: `sources/raw/channel-policy-packets/v1.0/01_CH01_BM1_DISTRIBUTION_REVENUE_PACKET.md`
- Charter source SHA-256: `18203214a65639f5d07b498a41f03774c6849402d3cb46f05d5a371ca048b064`
- Source baseline: `COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE`
- Supporting baseline: STEP 3–5 `OWNER-REVIEW CANDIDATE`
- Overall classification: `B. SELECTIVE FIT — CANDIDATE`
- Date (KST): `2026-08-29`

This charter is derived from the exact standalone policy packet above. The raw packet preserves authoritative wording. Channel conclusions are Candidate inputs until the required CH-00 and Owner stages occur.

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

Next Owner review: when `BM1-DIST-02` through `BM1-DIST-06` Candidates close and an MVP selection/economic judgment is required.

## Four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

CH-01 owns specialist work for BM1; it does not change the order or create a fifth BM.

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

Primary question: what Interchain Asset Distribution Market product will issuers repeatedly pay for, and how can its outcomes and external revenue be proven in a manipulation-resistant way?

Mission: close Campaign contracts, attribution, anti-gaming, provider payout, Revenue Events, and recurring external-revenue evidence without making BM1 dependent on prior AI-routing success.

## Scope

In scope:

- Issuer Campaign registration, budget, duration, and target definition.
- Provider, wallet, DEX, bridge, and analytics actor roles.
- Campaign baseline and incremental performance.
- Time-weighted balance, verified holder, liquidity depth, retention.
- 30/60/90-day performance windows.
- Wash transfer, self-dealing, circular-flow, and sybil controls.
- Attribution sources and independent calculation.
- Provider payout, holdback, clawback, and dispute.
- Revenue Event and Revenue Vault linkage.
- Separation of contracted, accrued, and received revenue.
- Separate evidence for ATOM purchase or Community Pool deposit.
- Willingness to pay, renewal, and unit economics.
- A 3–6 month Distribution MVP scope and Kill conditions.

Out of scope:

- AI route-model design.
- Live failover, split, or hedged execution.
- Final BM2 SLA metrics or breach rules.
- BM3 institution policy/API design.
- Final BM4 common registry schema.
- Final legal-party, tax, or accounting conclusions.
- A Hub-owned marketing agency or exclusive distribution operator.

## Local hard locks

- Do not make AI Routing success a BM1 start condition.
- Do not treat transaction volume or TVL growth alone as performance.
- Do not record internal token circulation or recycled subsidy as external revenue.
- Do not finalize payout from issuer/provider self-report alone.
- Define a baseline that separates Campaign performance from general market appreciation.
- Apply anti-gaming rules before payout and provide a post-payment clawback path.
- Separate Revenue Event states: `CONTRACTED`, `ACCRUED`, and `RECEIVED`.
- Mark ATOM purchase or Community Pool attribution realized only with actual transaction evidence.
- BM1 data may be reused by BM2/AI research, but that reuse must not dilute BM1 customer value.

## Canonical objects

- Distribution Campaign
- Issuer
- Campaign Budget
- Target Asset / Chain / Market
- Eligible Provider
- Attribution Event
- Performance Window
- Baseline
- Incremental Outcome
- Anti-gaming Flag
- Payout Record
- Holdback / Clawback
- Revenue Event
- Revenue Vault Reference
- Campaign Receipt

## Minimum performance frame

1. Baseline: pre-Campaign state and natural-growth trend.
2. Increment: additional outcome attributable to the Campaign.
3. Quality: real holders, depth, retention, and usability.
4. Integrity: exclude wash, self-dealing, and circular flows.
5. Economics: `issuer payment - provider payout - operating cost = protocol contribution`.
6. Persistence: renewal and 30/60/90-day retention.

## Dependencies and interfaces

- Input from CH-02: verifiable events, timestamps, provenance, and receipt semantics.
- Input from CH-06: provider capabilities and factual history.
- Input from CH-07: contracting parties, payout/clawback, revenue recognition, and competition boundary.
- Output to CH-02: telemetry and evidence requirements for Campaign attribution.
- Output to CH-06: Campaign-provider capability and performance-history Candidates.
- Output to CH-00: Decision Handoff affecting the BM1 MVP, revenue definition, or commercial roadmap.

AI/6G is not a BM1 dependency. The current roadmap says BM1 remains commercial-first and uses the evidence foundation as support.

## Required outputs

- `BM1-DIST-01`: CURRENT_MARKET_AND_ACTOR_BASELINE
- `BM1-DIST-02`: DISTRIBUTION_CAMPAIGN_OBJECT_AND_FLOW
- `BM1-DIST-03`: ATTRIBUTION_AND_ANTI_GAMING_SPEC
- `BM1-DIST-04`: PROVIDER_PAYOUT_HOLDBACK_CLAWBACK_RULE
- `BM1-DIST-05`: REVENUE_EVENT_AND_VAULT_EVIDENCE_MODEL
- `BM1-DIST-06`: DISTRIBUTION_MVP_AND_WTP_GATE

## Decision questions

- What outcome does an issuer buy?
- How is incremental attribution proven?
- When does provider payout become final?
- Which gaming signals trigger holdback or clawback?
- What minimum state belongs on Hub/CosmWasm, and what calculation stays off-chain?
- How is actual external revenue traced to the Revenue Vault?
- What single customer value must the 3–6 month MVP validate?

## Pass, hold, and kill/pivot

Pass when the paid outcome is intelligible, attribution/anti-gaming is independently reproducible, payout and revenue states are separated, external paid revenue and renewal evidence exist, and the MVP works without AI.

Hold when the baseline is unstable or independently uncomputable, payout depends too heavily on provider self-report, or interest exists without price/contract/renewal evidence.

Kill/pivot when paid demand repeatedly fails, no material performance remains after gaming removal, measurement/provider/operations cost persistently exceeds gross revenue, or the model collapses into subsidy allocation/internal token circulation.

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

Define the Campaign Product and Revenue Evidence first; do not lead with AI or 6G. No production, implementation, live financial execution, commercial SLA, native module, fifth BM, or full v1.2 rewrite is authorized.
