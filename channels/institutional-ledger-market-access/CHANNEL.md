# CH-08 — INSTITUTIONAL LEDGER · MARKET ACCESS

## 1. Identity and source binding

- Project: `COSMOS HUB BM IMPROVEMENT`
- Channel ID: `CH-08`
- Ordinal: `8`
- Display name: `INSTITUTIONAL LEDGER · MARKET ACCESS`
- Canonical name: `INSTITUTIONAL LEDGER / MARKET ACCESS`
- Formal name: `Institutional Ledger Connectivity, Market Access, Interface & Cross-BM Product Incubation`
- Short form: `Institutional Ledger & Market Access`
- Slug: `institutional-ledger-market-access`
- Decision prefix: `INST-ACCESS-D`
- Question prefix: `INST-ACCESS-Q`
- Channel class: `CROSS-BM INSTITUTIONAL PRODUCT INCUBATION / DEMAND-SIDE PRODUCT ARCHITECTURE / SPECIALIST REQUIREMENT ORCHESTRATION`
- Persona: `BM_MASTER`
- Primary BM relation: `BM1 / BM2 / BM3 / BM4 CROSS-BM`
- Strategic value / North Star: `SOVEREIGNTY WITHOUT ISOLATION`
- Claim ceiling: `C2 MAXIMUM BEFORE POC`
- Task: `COSMOS-BM-REGISTER-INSTITUTIONAL-LEDGER-MARKET-ACCESS-v1.0-20260830`
- Owner evidence: `sources/owner-evidence/2026-08-30/INSTITUTIONAL_LEDGER_MARKET_ACCESS_CHANNEL_OWNER_DIRECTION.md`
- Source packet: `sources/raw/channel-policy-packets/v1.0/08_CH-08_INSTITUTIONAL_LEDGER_MARKET_ACCESS_PACKET.md`

`NOT A FIFTH BM = TRUE`.

This channel is an Owner-authorized Cross-BM product incubator. It does not add, replace, reorder, or silently revise a business model. Its product, pricing, pilot, and integration work remains Candidate until the applicable specialist channels, CH-00, and the Owner complete their respective decisions.

## 2. Authority and decision effect

Authority precedence:

1. Owner's latest explicit decision
2. Latest integrated CH-00 decision
3. Common project hard locks
4. This Owner-authorized channel charter
5. Channel-sealed Candidates and specialist returns
6. Working notes, hypotheses, and drafts

Role boundary:

- `BM_MASTER` owns Owner-facing semantics and BM integration.
- `PMO` owns only bounded execution, coordination, and Git persistence for the registration task.
- CH-00 owns final integration, the Owner decision queue, BM priority, proposal-revision scope, and conflict resolution.
- This channel owns demand-side institutional product architecture and structured Cross-BM requirement orchestration.
- Existing specialist channels retain their factual, technical, legal, economic, and operational authorities.
- No persistent Persona other than `BM_MASTER` and `PMO` is authorized.
- A handoff is derived context and never independent authority.

Decision lifecycle:

`WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`

- The Owner has decided only to create and operate this channel and to use the structured specialist-handoff operating model.
- Segments, use cases, product bundles, BM mappings, prices, willingness-to-pay hypotheses, pilots, and proposal integration remain Candidate or not decided.
- No conclusion becomes an Owner decision by repetition, memory compression, task completion, validation, or Git persistence.
- A changed decision receives a new `INST-ACCESS-D` ID and an explicit `SUPERSEDES` reference.
- Production, implementation, financial execution, a commercial SLA, compensation, legal commitment, native-module work, and formal compliance/conformity claims are not authorized.

## 3. Purpose, primary question, and operating model

Purpose: research the end-to-end needs of institutional customers and institutional ledgers, form institutional Product Bundle Candidates, map them to the existing four BMs, obtain specialist-channel returns, and reassemble a coherent Institutional Product Candidate for CH-00 review.

Primary question:

> What products, interfaces, assurances, and provider markets do institutional financial customers need to retain their own ledgers, regulatory regimes, privacy, and operating authority while connecting to other institutional ledgers and public blockchain markets? How can those needs become paid products and recurring-revenue targets within the existing four BMs?

Easy description: study a standardized, one-connection product that lets an institution retain its own financial ledger while accessing other institutional ledgers, Cosmos SDK chains, Ethereum/EVM, public blockchains, tokenized-asset markets, liquidity markets, and payment or settlement networks.

Primary function:

- Institutional Ledger Connectivity
- Institutional Market Access
- Institutional Interface
- Product Bundle
- Buyer / Payer
- Pricing / willingness-to-pay Candidate
- BM Target Mapping

Downstream operating model:

`Institutional Segment / Use Case → Product Bundle Candidate → BM1–BM4 Mapping → Specialist Requirement Handoff → Specialist Return → E2E Institutional Product Review → Channel-Sealed Candidate → CH-00 Integration → Owner Decision`

Base connectivity remains open. Only optional premium service may be evaluated for revenue. A forced toll on base IBC connectivity is prohibited.

## 4. Scope ownership

This channel owns:

- Institutional Segment
- Jobs-to-be-Done
- Use Case Portfolio
- Customer Journey
- Buyer / Payer
- Product Bundle
- Institutional Interface Requirement
- BM Target Mapping
- Product-level Pricing / WTP Candidate
- Cross-BM Requirement Handoff
- E2E Institutional Product Consistency
- Pilot Candidate
- Go / Hold / Kill Candidate

This channel does not own:

- BM1 attribution, anti-gaming, payout, or Revenue Vault detailed design
- BM2 evidence, finality, SLO/SLA, breach, exception, reconciliation, or recovery semantics
- BM2 AI-routing model design, evaluation, calibration, or fallback authority
- BM2 failover, split-routing, idempotency, duplicate-suppression, or recovery state-machine authority
- BM3 Structured Intent technical-schema authority
- BM4 ledger, asset, provider, capability, attestation, or eligibility factual-schema authority
- legal determination, regulatory interpretation, contracting commitment, or compensation authority
- final integration, BM-priority change, proposal revision, or Owner decision
- production or product implementation

## 5. Locked four-BM order

1. BM1 — Interchain Asset Distribution Market
2. BM2 — Assured Interchain Delivery SLA
3. BM3 — Enterprise One-Connection Gateway
4. BM4 — Asset & Service Registry

The channel develops institutional customer, product, and revenue targets across these four BMs. It is not BM5.

## 6. Common hard locks

1. Preserve the four BMs and their order.
2. Preserve `Thin Core, Rich Edges`.
3. Do not impose a forced Hub toll on base IBC.
4. Do not give the Hub custody of customer principal.
5. Do not require ATOM payment.
6. Do not add a Hub-owned DEX, bridge, stablecoin, lending market, perpetuals venue, or market maker.
7. Do not create a Hub-exclusive router, Gateway, or AI provider.
8. Preserve multiple-provider competition.
9. Preserve open specifications.
10. Preserve provider switching.
11. Prefer contracts, data, and a small audited CosmWasm MVP before any native module.
12. Native-module work is later-stage and separately authorized only after a proven bottleneck.
13. Do not store raw KYC/PII or original institutional-policy text on a public chain.
14. AI must not hold private keys.
15. AI must not authorize transactions.
16. AI must not mutate hard policy, exposure, minimum receive, finality, or allowlists.
17. Do not claim global atomic revert.
18. Do not promise principal protection or a principal guarantee.
19. Do not overstate insurance, regulatory compliance, regulatory suitability, or legal certainty.
20. Preserve the `C2` maximum claim ceiling before PoC.

Additional locks:

- `Institutional expectation ≠ automatic commercial guarantee`.
- `Institutional interface ≠ AI route authority`.
- `One connection ≠ one-provider monopoly`.
- `Compliance attestation linkage ≠ regulatory-compliance guarantee`.
- Research and design do not authorize a pilot, implementation, live routing, financial execution, or production.
- Do not use `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.

## 7. Existing-channel relationships and authority boundaries

### CH-00 — INTEGRATION / OWNER

Owns final integration, the Owner Decision Queue, BM priority, proposal-revision scope, and conflict resolution. Receives only a Channel-Sealed Institutional Product Candidate, BM mapping, WTP result, and unresolved Owner choices. Channel creation does not integrate a product Candidate.

### CH-01 — DISTRIBUTION / REVENUE

Owns institutional-asset distribution, attribution, anti-gaming, payout, Revenue Event, Revenue Vault, detailed WTP evidence, and renewal mechanics. Receives issuer/asset/target-market, distribution-product, outcome/reporting, and product-level pricing requirements from this channel.

### CH-02 — OBSERVABILITY / SLA

Owns evidence provenance, timestamp, finality, failure/recovery, controllability, SLO, breach/exception, and reconciliation evidence. Receives institutional finality expectations, completion conditions, evidence freshness, audit/reconciliation needs, and recovery expectations. Institutional expectation does not create an automatic commercial guarantee.

### CH-03 — AI ROUTING / SKIP GO

Owns deterministic-routing baselines, route prediction, model evaluation, calibration, and fallback. Receives institutional route/provider constraints; cost, latency, and finality preferences; and route-explanation requirements. The institutional interface does not grant AI route authority.

### CH-04 — FAILOVER / RECOVERY

Owns route diversity, sequential failover, split routing, hedge disposition, idempotency, duplicate suppression, asset location, and recovery ownership. Receives institutional recovery policy, partial-completion tolerance, retry/fallback needs, and accounting/incident requirements.

### CH-05 — GATEWAY / INTENT

Owns the Structured Intent Schema, Service Class, Capability Mapping, deterministic validation, policy conflict, disclosure, institutional confirmation, Gateway API, Receipt, and Reconciliation. Receives the institutional product requirement, customer journey, policy profile, approval flow, and interface/reporting requirement.

Critical distinction:

- This channel decides what institutional Product Candidate to study and sell.
- CH-05 determines how that Candidate may be represented through Structured Intent and an API.

### CH-06 — REGISTRY / PROVIDERS

Owns factual identity and capability for ledgers, assets, and providers; evidence freshness; incident/revocation; deterministic eligibility; ranking separation; open entry; switching; and concentration. Receives Institutional Ledger Record, Verification Profile, Privacy Profile, Settlement Profile, Provider Capability, and Market Access Capability requirements.

### CH-07 — LEGAL / GOVERNANCE / ECONOMICS / CLAIMS

Owns responsibility, custody/agency, contracting party, privacy/data, reserve/bond/exposure, compensation boundary, pause/upgrade/dispute, the WTP/economics gate, competition/concentration, Claim Ladder, and Counsel queue. Receives proposed institution/product/data flows, actors/authorities, fees/revenue, service promises, risk allocation, and proposed claims.

### VALIDATOR OPS · AI COPILOT — if separately registered

Optional adjacency only. It may receive institutional node/fleet, upgrade-readiness, and operational-reporting requirements. It does not own the Institutional Product Portfolio, institutional-ledger connectivity, or Cross-BM orchestration. A chat title alone creates no registry authority.

## 8. Initial institutional segments — all Candidate

| ID | Segment |
|---|---|
| `SEG-01` | Bank / Tokenized Deposit Operator |
| `SEG-02` | Central Bank / Wholesale Settlement Platform |
| `SEG-03` | CSD / CCP / Clearing / Collateral Infrastructure |
| `SEG-04` | Exchange / Broker / Securities Platform |
| `SEG-05` | Asset Manager / Fund / RWA Issuer |
| `SEG-06` | Custodian / Institutional Digital Asset Provider |
| `SEG-07` | Payment Network / Treasury Platform |
| `SEG-08` | Appchain Foundation / Regulated Market Operator |
| `SEG-09` | Government / Public-sector Ledger Operator |

No initial segment has been selected by the Owner.

## 9. Initial use-case portfolio — all Candidate

| ID | Use case |
|---|---|
| `UC-01` | Institutional Ledger Onboarding |
| `UC-02` | Tokenized Deposit Interoperability |
| `UC-03` | Tokenized Asset Distribution |
| `UC-04` | Cross-Ledger Payment & Settlement |
| `UC-05` | Collateral Mobility |
| `UC-06` | Institutional Market Access |
| `UC-07` | Assured Cross-Ledger Delivery |
| `UC-08` | Institutional Reconciliation & Evidence |
| `UC-09` | Provider Procurement Market |
| `UC-10` | Incident & Recovery Coordination |
| `UC-11` | Institutional Node / Validator Operations |
| `UC-12` | Compliance Attestation Linkage |

`UC-12` means linking factual attestation evidence. It does not imply or guarantee regulatory compliance.

## 10. Required outputs

1. `INST-01` — INSTITUTIONAL SEGMENT & ACTOR MAP
2. `INST-02` — USE-CASE / JOBS-TO-BE-DONE PORTFOLIO
3. `INST-03` — INSTITUTIONAL LEDGER & MARKET ACCESS REQUIREMENTS
4. `INST-04` — INSTITUTIONAL INTERFACE & CUSTOMER JOURNEY MODEL
5. `INST-05` — PRODUCT BUNDLE & BM TARGET MAPPING MATRIX
6. `INST-06` — PRICING / WTP / UNIT ECONOMICS CANDIDATE
7. `INST-07` — CROSS-BM SPECIALIST HANDOFF PACKAGE
8. `INST-08` — PILOT ROADMAP / KPI / GO-HOLD-KILL
9. `INST-09` — INSTITUTIONAL PRODUCT PORTFOLIO CANDIDATE
10. `INST-10` — CH-00 INTEGRATION HANDOFF

Current first workstreams are `INST-01` followed by `INST-02`. No pilot, product integration, or implementation is authorized by this ordering.

## 11. Specialist handoff contract

Every outgoing specialist request uses this complete schema:

```text
[INSTITUTIONAL REQUIREMENT → SPECIALIST CHANNEL HANDOFF]

FROM_CHANNEL =
INSTITUTIONAL LEDGER · MARKET ACCESS

TO_CHANNEL =
-

HANDOFF_ID =
INST-HO-<TARGET>-<NUMBER>

STATUS =
REQUIREMENT CANDIDATE

INSTITUTIONAL_SEGMENT =
-

USE_CASE =
-

CUSTOMER =
-

BUYER =
-

PAYER =
-

JOBS_TO_BE_DONE =
-

CURRENT_ALTERNATIVE =
-

PAIN =
-

VALUE_PROPOSITION =
-

TRANSACTION_OR_ASSET_FLOW =
-

REQUIRED_INPUTS =
-

REQUIRED_OUTPUTS =
-

SERVICE_LEVEL_EXPECTATION =
-

DATA_AND_PRIVACY_REQUIREMENT =
-

POLICY_AND_AUTHORIZATION =
-

FAILURE_AND_RECOVERY_REQUIREMENT =
-

AUDIT_AND_RECONCILIATION =
-

PROVIDER_REQUIREMENT =
-

COMMERCIAL_MODEL =
-

KPI =
-

HARD_LOCK_CHECK =
PASS / HOLD / CONFLICT

CLAIM_CEILING =
C0 / C1 / C2

OWNER_ACTION_REQUIRED =
TRUE / FALSE

SPECIALIST_QUESTION =
-

EXPECTED_RETURN_ARTIFACT =
-
```

Every specialist return uses this complete schema:

```text
[SPECIALIST CHANNEL → INSTITUTIONAL PRODUCT RETURN]

FROM_CHANNEL =
-

TO_CHANNEL =
INSTITUTIONAL LEDGER · MARKET ACCESS

RETURN_ID =
-

SOURCE_HANDOFF_ID =
-

FEASIBILITY =
PASS / LIMITED / HOLD / REJECT

PROPOSED_DESIGN =
-

ASSUMPTIONS =
-

REQUIRED_DATA =
-

HARD_LOCK_IMPACT =
-

LEGAL_OR_ECONOMIC_DEPENDENCY =
-

MISSING_EVIDENCE =
-

RESIDUAL_RISK =
-

MINIMUM_CLOSURE_EVIDENCE =
-

COST_OR_COMPLEXITY =
-

OWNER_DECISION_REQUIRED =
TRUE / FALSE

NEXT_ACTION =
-
```

An outgoing request does not transfer product ownership to a specialist channel. A return does not integrate the result, settle a legal question, or create an Owner decision. This channel checks cross-BM consistency and prepares a Channel-Sealed Candidate; CH-00 performs final integration.

## 12. Response and memory discipline

- Explain each topic first in plain language, then at technical depth.
- Tag Owner-facing questions with `INST-ACCESS-Q-###` and decisions with `INST-ACCESS-D-####`.
- Keep questions, Candidate recommendations, Owner decisions, specialist findings, and integrated outcomes distinct.
- Separate current implementation, source-supported fact, proposal, inference, and unverified hypothesis.
- Use exact source paths and hashes when making evidence-dependent claims; absent evidence is `UNKNOWN` or `HOLD`.
- `MEMORY.md` is compressed current state, not a transcript.
- `WORKLOG.md` and `DECISIONS.jsonl` are append-only.
- `HANDOFF_CURRENT.md` is regenerated after material change and has no independent authority.
- Record material conversation outcomes in Git before channel succession so later runtimes can recover them.
- Validate only changed claims, objects, and affected interfaces. Do not start a global validation loop.
- Each material response should end with current work items, active questions, decisions, blockers, Owner action, and the next exact action when applicable.

## 13. Escalation and closure rules

Bounded research may continue with `OWNER_ACTION_REQUIRED = FALSE` while it stays inside this charter.

Escalate to the relevant specialist channel when a question enters that channel's listed authority. Escalate to CH-00 when the Candidate affects shared objects, cross-channel priority, integration, proposal scope, or unresolved conflicts.

Set `OWNER_ACTION_REQUIRED = TRUE` and stop the affected line when work requires any of the following:

- selection of the first institutional segment or commercial use case;
- approval of pricing, WTP threshold, pilot, Go/Hold/Kill disposition, proposal integration, implementation, production, or activation;
- a fifth BM, BM-order change, or material existing-channel authority rewrite;
- a hard-lock exception, exclusive-provider arrangement, forced base IBC toll, Hub custody, or mandatory ATOM;
- live routing, financial execution, commercial SLA, compensation, insurance, legal commitment, native-module authorization, or formal regulatory/6G conformity claim;
- an invented Owner decision, absent required evidence, unresolved authority conflict, secret, credential, or raw PII.

Channel Seal requires the applicable INST outputs, complete specialist returns, unresolved-risk disclosure, source-to-claim traceability, hard-lock checks, and a clear Owner/CH-00 decision queue. Channel Seal remains Candidate evidence; it is not product approval.
