# CH-07 — LEGAL / GOVERNANCE / ECONOMICS / CLAIMS

## 1. Identity and exact source binding

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-07`
- Canonical slug: `legal-governance-economics`
- Decision prefix: `LGEC-D`
- Role: Cross-cutting Legal / Governance / Economics / Claim Gate Channel
- Packet type: Cross-cutting gate / responsibility / governance / economics / claim management / no product redesign
- Effective packet date: `2026-08-29 KST`
- Exact charter source: `sources/raw/channel-policy-packets/v1.0/07_CH07_LEGAL_GOVERNANCE_ECONOMICS_CLAIMS_PACKET.md`
- Exact charter SHA-256: `fc27c08c370ebcd181b23f17300da954e430efa7a8f9b2f933f626e3cc1ab151`

This file is a faithful Git charter derived from the corrected standalone packet above. It does not use the older archived E02 copy as authority.

## 2. Authority, decision effect, and current authorization

Authority precedence:

1. Owner's latest explicit decision
2. Latest integrated decision from `CH-00 INTEGRATION / OWNER DECISIONS`
3. Common hard locks in this charter
4. Local hard locks and channel-sealed decisions
5. Working notes, hypotheses, and drafts

Decision lifecycle:

`WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`

- Channel conclusions are `CANDIDATE` by default.
- They are not project decisions before CH-00 integration and any required Owner decision.
- This channel does not silently alter another channel's scope, authority, or object definitions.
- A changed decision requires a new `LGEC-D` ID and an explicit `SUPERSEDES` reference.
- `OWNER_ACTION_REQUIRED = FALSE` for bootstrap, investigation, and design discussion.
- `OWNER_ACTION_REQUIRED = TRUE` only for an Owner choice, common-boundary change, proposal-text integration, pilot, implementation, external counsel engagement, or other separately gated action.
- Next Owner review: when LGEC-01 through LGEC-06 identify the items requiring Owner selection, external counsel, or a pilot gate.

Current authorization state:

- Production: `NOT AUTHORIZED`
- Full v1.2 rewrite: `NOT AUTHORIZED`
- New/fifth BM: `NOT AUTHORIZED`
- Native module design: `NOT AUTHORIZED`
- Live routing or financial execution: `NOT AUTHORIZED`
- Commercial SLA or compensation: `NOT AUTHORIZED`
- Formal 6G conformity claim: `NOT AUTHORIZED`

The v1.1 proposal is an independent `CANDIDATE`, not official Cosmos Hub policy. STEP 3–5 is an `OWNER-REVIEW CANDIDATE`. The overall classification `B. SELECTIVE FIT` and all concept dispositions remain `CANDIDATE`. `OR-01` through `OR-09` are `UNDECIDED` and must not be inferred from their recommendations.

## 3. Four-BM order — locked

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

The count, names, and priority order are unchanged.

## 4. Common hard locks

- Preserve `Thin Core, Rich Edges`.
- Base IBC remains open; no forced Hub toll is imposed on base IBC.
- The Hub does not custody customer principal.
- ATOM is not a mandatory payment asset.
- Do not add a Hub-owned DEX, bridge, lending market, perpetuals venue, stablecoin, market maker, or proprietary mandatory router.
- Do not put raw KYC/PII or an institution's sensitive policy text on a public chain.
- Validate contracts and data, then a small audited CosmWasm MVP, before any native module.
- A native module may be considered only after a real repeated-operational bottleneck is proven and the Owner separately approves it.
- AI does not hold private keys or authorize transactions.
- AI does not mutate hard policy, exposure caps, minimum receive, finality, or allowlists.
- AI does not decide compensation, disputes, or legal responsibility unilaterally.
- Do not imply global atomic revert, principal guarantee/protection, insurance, or regulatory suitability/compliance.
- Preserve open provider competition, public specifications, switching, and no exclusive mandatory operator.
- Do not use `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.
- The roadmap is a selective prior-art adaptation candidate, not a production architecture approval.

## 5. Status vocabulary

- `CURRENT IMPLEMENTATION`: actually exists in Cosmos/IBC/Skip/Wallet/Indexer today.
- `EXISTING / PARTIAL`: exists only in a narrower or limited form.
- `SOURCE-SUPPORTED FACT`: directly supported by a cited primary source.
- `OFFICIAL ROADMAP / CONTRACTUAL ANNOUNCEMENT`: official direction or announced contract; not the same as operation or realized revenue.
- `V1.2 CHANNEL CANDIDATE`: proposed here but not integrated.
- `SELECT-LIMITED RESEARCH ITEM`: may proceed only behind hard gates.
- `WATCH`: independent research awaiting evidence.
- `REJECTED BY GOVERNANCE`: excluded by a hard lock or selection result.
- `OWNER DECISION REQUIRED`: cannot be finalized by this specialist channel.
- `CH-00 INTEGRATION REQUIRED`: changes shared objects, priorities, or channel interfaces.

## 6. Primary question and mission

Primary question: can a technically possible Candidate become an executable product when legal responsibility, governance authority, economics, neutrality, and claim strength are considered?

Mission:

- Do not redesign another channel's product.
- Give each Candidate explicit responsibility, authority, exposure, revenue, and claim `GO / HOLD / KILL` conditions.
- Produce boundary memos that let the Owner and CH-00 make an integration decision.
- Keep every conclusion bounded, evidence-linked, non-official, and below its actual maturity.

## 7. Scope

In scope:

- responsibility separation among Router, Provider, Gateway, Wallet, Hub, and Evidence Operator;
- contract party, invoice path, and revenue flow;
- custody, agency, and discretionary-execution boundaries;
- responsibility for an incorrect recommendation or policy translation;
- provider-controllable breach versus external event;
- Provider Bond, reserve, exposure cap, and compensation ceiling;
- boundary between SLA and guarantee/insurance;
- partial completion, duplicate execution, recovery liability, and capital lock;
- data privacy, PII, institution policy, and trade secrets;
- AI model responsibility, explainability, discrimination, and concentration;
- open provider competition and proprietary-data lock-in;
- governance authority over admin keys, pause, upgrade, revocation, and disputes;
- willingness to pay, unit economics, support and incident cost;
- contracted, accrued, and received revenue as distinct states;
- evidence for ATOM purchase and Community Pool deposit;
- Claim Ladder C0–C5 and wording allowed per document/channel;
- adversarial review and residual risk;
- a bounded list of questions requiring external counsel or audit.

Out of scope:

- designing BM1's campaign product;
- writing BM2 telemetry, models, or state machines;
- writing BM3 API/UX;
- selecting BM4 factual fields in place of CH-06;
- claiming a legal opinion, regulatory approval, or insurance authorization already exists;
- entering a production contract;
- drafting language that guarantees investment returns, delivery, or principal.

## 8. Local hard locks

- Before legal review, do not describe compensation as insurance or a guarantee.
- Do not impose unlimited responsibility for events that are not technically controllable.
- A commercial pilot cannot pass without bounded exposure, reserve/bond, and payout ceiling.
- Do not assume a `non-custodial` label alone removes custody or agency risk.
- Separate responsibility for a model recommendation from final authorization.
- Test whether provider ranking increases discrimination or market concentration.
- Keep raw PII/KYC and institution policy off public chain.
- Distinguish revenue announcement from actual received external inflow.
- 6G, AI, and SLA wording must not exceed source status or measured maturity.
- Mark questions needing a formal legal conclusion as `COUNSEL REQUIRED`.
- Return exact HOLD conditions and minimum closure evidence; do not block indefinitely with a generic objection.

## 9. Claim ladder and wording boundary

| Level | Meaning | Current use |
|---|---|---|
| C0 | Internal hypothesis | Allowed when labeled |
| C1 | Structural similarity/alignment | Allowed when sourced |
| C2 | Selective design informed by official research | Current maximum before PoC |
| C3 | Applied and measured in a bounded PoC | Not yet available |
| C4 | Exact-scope operating pilot | Not yet available |
| C5 | Actual conformity assessment/certification | Unavailable in this programme |

Pre-PoC examples permitted at or below C2 include `6G-era network-orchestration research-informed`, `selected autonomous-network management principles adapted to Interchain`, and `bounded AI-assisted Interchain orchestration roadmap`.

Prohibited without the exact later evidence and authority:

- `6G Blockchain`, `6G-compliant Cosmos Hub`, `6G-certified Interchain`, `First 6G Chain`, `IMT-2030 compliant`, `3GPP 6G implemented`;
- `Guaranteed Delivery`, `Risk-free Provider`, `Global Atomic Revert`, `Principal Protection`;
- `Insurance-backed` without an actual authorized insurance/legal/contract basis.

## 10. Responsibility questions

- Who issues the quote and who constructs the execution plan?
- Who approves route policy and who signs the transaction?
- Who gathers evidence and who adjudicates a breach?
- Who performs recovery and bears its cost?
- Who pays compensation and what is the maximum exposure?
- Do Hub/CosmWasm provide rules and references only, or become a contracting party?
- How is protocol share attributed from enterprise-operator revenue?
- Who controls pause, upgrade, keys, revocation, and dispute resolution?

## 11. Dependencies and outputs

Inputs:

- CH-01: campaign contract, payout, clawback, revenue flow, willingness to pay;
- CH-02: measurable breach, exceptions, and evidence authority;
- CH-03: model role, calibration, discrimination, concentration, and operating cost;
- CH-04: duplicate execution, partial legs, recovery, capital lock, and accounting risk;
- CH-05: institution authorization, data, custody/agency, and support responsibility;
- CH-06: attestation, factual labels, provider neutrality, and revocation.

Outputs:

- To every channel: `GO / HOLD / KILL` boundary, residual risk, claim ceiling, and Owner issues.
- To CH-00: integrated legal-governance-economic recommendation and revision-scope constraints.

Required artifacts:

1. `LGEC-01` — LEGAL_BOUNDARY_AND_RESPONSIBILITY_MATRIX
2. `LGEC-02` — GOVERNANCE_AUTHORITY_PAUSE_UPGRADE_DISPUTE_MAP
3. `LGEC-03` — ECONOMIC_VIABILITY_RESERVE_EXPOSURE_MODEL
4. `LGEC-04` — CLAIM_LADDER_AND_CHANNEL_CLAIM_REGISTER
5. `LGEC-05` — INTEGRATED_ADVERSARIAL_FINDINGS
6. `LGEC-06` — COUNSEL_AUDIT_AND_OWNER_DECISION_ISSUE_LIST

Current start point: freeze LGEC-01 and LGEC-04 first.

## 12. GO / HOLD / KILL

GO only when responsibility and controllable events are clear; amount, exposure, reserve, payout and pause are bounded; data and authority are least-privilege; willingness to pay and operating economics are plausibly positive; provider competition and switching remain; and claims match evidence maturity.

HOLD when a legal party, insurance/custody/agency issue, privacy classification, governance key/pause/upgrade/dispute authority, support/incident/compensation cost, or source-to-public-wording match remains unresolved.

KILL / REJECT when exposure is unbounded relative to revenue; the product requires Hub custody, guarantee, exclusive operation, or uncontrolled provider discrimination; exaggerated principal/insurance/regulatory/6G language is essential to the value proposition; or financial rights must be executed automatically without exact evidence.

Every review returns:

```text
OBJECTION =
EVIDENCE =
RESPONSE =
RESIDUAL RISK =
MINIMUM CLOSURE EVIDENCE =
ROADMAP IMPACT =
GO / HOLD / KILL =
```

## 13. Validation, handoff, and reporting

- Validate only changed claims, objects, and affected interfaces.
- Do not create a full re-research, global regression, or repeated validation loop.
- Separate fact, proposal, inference, and unverified hypothesis.
- Attach `SOURCE CLASS`, `IMPLEMENTATION STATUS`, and `CLAIM CEILING` where needed.
- If evidence is absent, record `UNKNOWN` or `HOLD`; do not fill the gap by inference.
- Bind PASS to the exact document, schema, data, code, or contract scope.
- Failure of one optional track does not automatically invalidate unrelated tracks.

CH-00 handoff fields:

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

Do not send only a narrative summary. Separate decision, evidence, impact, and unresolved issues. Use Decision IDs rather than repeated manual explanation. CH-00 registers cross-channel dependencies.

Channel reports use:

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
