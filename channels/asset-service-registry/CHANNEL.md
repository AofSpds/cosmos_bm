# CH-06 — ASSET & SERVICE REGISTRY

## 1. Identity and exact source binding

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-06`
- Canonical slug: `asset-service-registry`
- Decision prefix: `BM4-REG-D`
- Role: BM4 Factual Registry / Open Provider Market / Neutrality Channel
- Packet type: factual registry / open provider market / neutrality / conflict arbitration / no approval badge
- Effective packet date: `2026-08-29 KST`
- Exact charter source: `sources/raw/channel-policy-packets/v1.0/06_CH06_BM4_REGISTRY_PROVIDER_MARKET_PACKET.md`
- Exact charter SHA-256: `17cb30af452ec3eb38b878d20503fccc01766b5bed189730f41e317600a7c437`

This charter is derived from the corrected standalone packet. The older archived E02 copy is not authority.

## 2. Authority, decision effect, and authorization

Authority precedence:

1. Owner's latest explicit decision
2. Latest integrated CH-00 decision
3. Common hard locks
4. Local hard locks and channel-sealed decisions
5. Working notes, hypotheses, and drafts

Decision lifecycle: `WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`.

- Every channel conclusion is Candidate by default; no project decision exists before CH-00 integration and any required Owner choice.
- Do not silently change another channel's scope, authority, or object definitions.
- A changed decision gets a new `BM4-REG-D` ID and `SUPERSEDES`.
- Owner action is not required for bounded bootstrap/investigation/design; it is required for Owner choice, common-boundary change, proposal integration, pilot, implementation, or operator/governance selection.
- Next Owner review: after BM4-REG-01 through BM4-REG-06 Candidate work closes and shared objects, neutrality controls, or Registry scope need selection.

Current authorization:

- Production, full v1.2 rewrite, new/fifth BM, native module design, live routing/financial execution, commercial SLA/compensation, and formal 6G conformity: `NOT AUTHORIZED`.

v1.1 is an independent proposal Candidate, not official Hub policy. STEP 3–5 is Owner-review Candidate. `B. SELECTIVE FIT` and all concept dispositions remain Candidate. OR-01–OR-09 are `UNDECIDED`.

## 3. Locked four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

## 4. Common hard locks

- Preserve `Thin Core, Rich Edges`.
- Base IBC remains open with no forced Hub toll.
- The Hub does not custody customer principal; ATOM is not mandatory payment.
- No Hub-owned DEX, bridge, lending market, perpetuals venue, stablecoin, market maker, or proprietary mandatory router.
- No raw KYC/PII or sensitive institution policy text on public chain.
- Contracts/data and a small audited CosmWasm MVP precede any native module; native design needs a proven bottleneck and separate Owner approval.
- AI does not hold keys, authorize transactions, mutate hard policy/exposure/minimum receive/finality/allowlists, or decide compensation/legal responsibility unilaterally.
- No global atomic revert, principal guarantee/protection, insurance, or regulatory suitability/compliance implication.
- Preserve open provider competition, public specifications, switching, and no exclusive mandatory operator.
- Do not use `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.
- Current roadmap is selective prior-art adaptation, not a production architecture approval.

## 5. Status vocabulary

- `CURRENT IMPLEMENTATION`: actually exists in Cosmos/IBC/Skip/Wallet/Indexer today.
- `EXISTING / PARTIAL`: a narrower or limited form exists.
- `SOURCE-SUPPORTED FACT`: directly supported by a cited primary source.
- `OFFICIAL ROADMAP / CONTRACTUAL ANNOUNCEMENT`: official direction or announced contract; not operation or realized revenue.
- `V1.2 CHANNEL CANDIDATE`: proposed here but not integrated.
- `SELECT-LIMITED RESEARCH ITEM`: may proceed only behind hard gates.
- `WATCH`: independent research awaiting evidence.
- `REJECTED BY GOVERNANCE`: excluded by a hard lock or selection result.
- `OWNER DECISION REQUIRED`: cannot be finalized by this channel.
- `CH-00 INTEGRATION REQUIRED`: changes shared objects, priorities, or interfaces.

A factual record or official announcement does not become a safety, approval, compliance, operation, or revenue claim.

## 6. Primary question and mission

Primary question: how can the system record, neutrally and verifiably, which asset/provider supports what, with which signature, evidence, performance, and incident history?

Mission: design Registry as a factual evidence interface—not an approval or guarantee badge. Keep provider eligibility, model ranking, open entry, switching, concentration, and conflict arbitration separate.

## 7. Scope

In scope:

- Asset Record and issuer-declared canonical representation/signature;
- issuer-labeled reserve/document/attestation pointer;
- Service Provider Record;
- Capability Record, supported routes/protocols, and signed quote reference;
- evidence freshness and revocation;
- historical latency/failure/recovery reference and incident history;
- SLA tier and bond reference;
- limited audit reference to model/version;
- deterministic eligibility versus provider ranking/confidence;
- open entry, switching, newcomer evaluation, and concentration KPI;
- self-reported telemetry discount/corroboration;
- conflict detection for capability, representation, or quote;
- deterministic arbitration and audit trail;
- minimum public/on-chain record versus detailed off-chain data.

Out of scope:

- `Hub Approved`, `Safe Asset`, `Guaranteed Provider`, or `Regulatory Compliant` badges;
- publishing raw KYC/PII, trade secrets, proprietary features, or model internals;
- operating a provider's route engine;
- AI-only eligibility decisions;
- a default or mandatory provider monopoly/router;
- replacing legal certification or licensing;
- Hub custody or direct competition with providers.

## 8. Local hard locks

- Record facts, signatures, sources, timestamps, and history only.
- Separate issuer-declared from independently verified.
- Separate provider self-report from independent evidence.
- Separate factual capability from performance score.
- Separate deterministic eligibility from model ranking.
- A score neither automatically ejects a provider nor grants an approval badge.
- Show confidence intervals, freshness, and missing data.
- Give newcomers an evaluation path so limited history is not permanent exclusion.
- Measure top-provider concentration and switching friction.
- Record incident scope, evidence, and resolution state.
- Keep detailed telemetry/sensitive data off-chain; place only minimum references on-chain.
- The Hub does not compete with providers or create a proprietary-data advantage.

Allowed factual labels:

`Supported Route`, `Signed Capability`, `Evidence Source`, `Evidence Freshness`, `Measured Historical Result`, `Attestation Issuer`, `Incident Record`, `Bond Reference`, `Revocation Status`, `Confidence / Missingness`.

Prohibited labels:

`Hub Approved`, `Safe Asset`, `Guaranteed Provider`, `Regulatory Compliant`, `Best Provider`, `Risk Free`, `Fully Verified`.

## 9. Minimum provider record and neutrality controls

Minimum provider record:

```text
provider_id
operator_identity_reference
service_types
supported_assets
supported_routes
supported_protocols
jurisdiction_or_policy_reference_if_disclosed
capability_signature
quote_interface
evidence_sources
telemetry_freshness
historical_result_reference
incident_reference
bond_reference
revocation_status
last_updated
schema_version
```

Neutrality controls:

- open capability and quote schema;
- multiple providers where the market permits;
- switching path;
- deterministic eligibility;
- ranking/eligibility separation;
- confidence and data-quality disclosure;
- top-provider share and concentration trend;
- newcomer evaluation quota/path;
- self-report corroboration;
- public conflict/arbitration rule;
- no exclusive mandatory operator.

## 10. Dependencies and outputs

Inputs:

- CH-01: distribution-provider roles and campaign-performance evidence;
- CH-02: canonical evidence, freshness, incident, and SLO/history semantics;
- CH-03: model confidence/version and separation from eligibility;
- CH-04: route/failover/split capability and recovery evidence;
- CH-05: capability-catalog and structured-intent mapping;
- CH-07: competition, discrimination, attestation, liability, and privacy boundary.

Output to CH-00: Candidate common Asset/Provider/Capability objects and neutrality decisions.

Required artifacts:

1. `BM4-REG-01` — ASSET_RECORD_AND_ISSUER_DECLARATION_SCHEMA
2. `BM4-REG-02` — PROVIDER_AND_CAPABILITY_RECORD_SCHEMA
3. `BM4-REG-03` — EVIDENCE_FRESHNESS_INCIDENT_REVOCATION_MODEL
4. `BM4-REG-04` — ELIGIBILITY_RANKING_AND_CONFIDENCE_SEPARATION
5. `BM4-REG-05` — OPEN_ENTRY_SWITCHING_CONCENTRATION_POLICY
6. `BM4-REG-06` — CONFLICT_DETECTION_AND_DETERMINISTIC_ARBITRATION

## 11. Questions and gates

Questions include the public-chain minimum factual record; issuer declaration versus external attestation; capability/history linkage; stale/conflicting evidence and revocation; eligibility/ranking separation; newcomer/dominant-provider feedback; and the Registry fields referenced by BM3.

PASS only when records bind signature/source/freshness/version; facts and opinions/rankings remain distinct; open entry and switching work; concentration/self-report dependence are measured; conflict resolution is deterministic and auditable; and no misleading label appears.

HOLD when the market is too thin, critical data is self-report-only, privacy/trade-secret boundaries are unclear, or scoring depends excessively on model estimates.

KILL/PIVOT when Registry becomes a perceived approval/guarantee authority, a provider becomes mandatory/exclusive, ranking creates an opaque monopoly feedback loop, switching fails, or raw PII/trade secrets are required.

Current start: close BM4-REG-01 through BM4-REG-03 factual schemas before score/ranking/market design.

## 12. Validation, claims, handoff, and reporting

- Validate only changed claims, objects, and affected interfaces; no full re-research, global regression, or repeated loop.
- Separate fact, proposal, inference, and unverified hypothesis.
- Attach source class, implementation status, and claim ceiling where needed.
- Missing evidence is `UNKNOWN` or `HOLD`; PASS is exact-scope-bound.
- One optional-track failure does not invalidate unrelated tracks.
- Current claim ceiling: `C2` before PoC.

CH-00 handoff fields: `FROM_CHANNEL`, `DECISION_ID`, `STATUS`, `QUESTION`, `RECOMMENDED_DECISION`, `ALTERNATIVES_CONSIDERED`, `EVIDENCE`, `RATIONALE`, `IMPACTED_CHANNELS`, `IMPACTED_BM`, `IMPACTED_TRACK`, `HARD_LOCK_CHECK`, `DEPENDENCIES`, `LEGAL_SAFETY_ECONOMIC_EFFECT`, `CLAIM_CEILING`, `OWNER_ACTION_REQUIRED`, `PROPOSED_INTEGRATION`, `SUPERSEDES`.

Channel reports use `OVERALL_PROGRESS`, `CURRENT_WORKSTREAM`, `CURRENT_QUESTION`, `CURRENT_BASELINE`, `MATERIAL_FINDINGS`, `DECISION_CANDIDATES`, `ALTERNATIVES`, `DEPENDENCIES`, `RISKS`, `BLOCKERS`, `OWNER_ACTION_REQUIRED`, and `NEXT_STEP`.
