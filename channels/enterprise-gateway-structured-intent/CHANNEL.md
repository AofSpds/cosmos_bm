# CH-05 — ENTERPRISE GATEWAY / STRUCTURED INTENT

## 1. Identity and exact source binding

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-05`
- Canonical slug: `enterprise-gateway-structured-intent`
- Decision prefix: `BM3-ENT-D`
- Role: BM3 Enterprise Product / Structured Intent / Capability Exposure Channel
- Packet type: enterprise product / structured intent / capability exposure / explicit authorization / no direct LLM execution
- Effective packet date: `2026-08-29 KST`
- Exact charter source: `sources/raw/channel-policy-packets/v1.0/05_CH05_BM3_ENTERPRISE_GATEWAY_INTENT_PACKET.md`
- Exact charter SHA-256: `ff46c3d8f1d2cc07e36f86559c4ed2afee728aaeb6c72e514719b632008860e2`

This charter is derived from the corrected standalone packet. The older archived E02 copy is not authority.

## 2. Authority, decision effect, and authorization

Authority precedence:

1. Owner's latest explicit decision
2. Latest integrated CH-00 decision
3. Common hard locks in this charter
4. Local hard locks and channel-sealed decisions
5. Working notes, hypotheses, and drafts

Decision lifecycle: `WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`.

- Every channel conclusion is `CANDIDATE` by default.
- No project decision exists before CH-00 integration and any required Owner choice.
- Do not silently alter another channel's scope, authority, or object definitions.
- A changed decision gets a new `BM3-ENT-D` ID and `SUPERSEDES`.
- Owner action is not required for bounded bootstrap/investigation/design; it is required for Owner choice, common-boundary change, proposal integration, pilot, implementation, or commercial commitment.
- Next Owner review: after BM3-ENT-02 through BM3-ENT-06 Candidate work closes and a pilot, service class, or proposal-integration choice is needed.

Current authorization:

- Production: `NOT AUTHORIZED`
- Full v1.2 rewrite: `NOT AUTHORIZED`
- New/fifth BM: `NOT AUTHORIZED`
- Native module design: `NOT AUTHORIZED`
- Live routing or financial execution: `NOT AUTHORIZED`
- Commercial SLA or compensation: `NOT AUTHORIZED`
- Formal 6G conformity claim: `NOT AUTHORIZED`

v1.1 is an independent `CANDIDATE`, not official Hub policy. STEP 3–5 is an `OWNER-REVIEW CANDIDATE`; `B. SELECTIVE FIT` and every portfolio disposition remain Candidate. OR-01–OR-09 remain `UNDECIDED`.

## 3. Locked four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

## 4. Common hard locks

- Preserve `Thin Core, Rich Edges`.
- Base IBC remains open with no forced Hub toll.
- The Hub does not custody customer principal.
- ATOM is not a mandatory payment asset.
- Do not add a Hub-owned DEX, bridge, lending market, perpetuals venue, stablecoin, market maker, or proprietary mandatory router.
- Do not put raw KYC/PII or sensitive institution policy text on public chain.
- Validate contracts/data and a small audited CosmWasm MVP before any native module; native design needs a proven bottleneck and separate Owner approval.
- AI does not hold keys, authorize transactions, mutate hard policy/exposure/minimum receive/finality/allowlists, or decide compensation/legal responsibility unilaterally.
- Do not imply global atomic revert, principal guarantee/protection, insurance, or regulatory suitability/compliance.
- Preserve open provider competition, public specifications, switching, and no exclusive mandatory operator.
- Do not use `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.
- This roadmap is a selective prior-art Candidate, not a production architecture approval.

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

Do not equate an official direction with operation/revenue or a Candidate with an implementation.

## 6. Primary question and mission

Primary question: what structured abstraction and operating product let an institution use policy-compatible Interchain services without manually composing chains, bridges, DEXs, and routers?

Mission: make One-Connection Gateway concrete through Structured Intent, Capability Catalog, Policy Adapter, Institutional Receipt, and Reconciliation. Natural language is an optional drafting interface only; it is never authoritative or a direct execution path.

## 7. Scope

In scope:

- enterprise customer problem and integration cost;
- Service Intent schema, Service Class, Policy Profile, Route Constraint, SLA Template reference, Receipt Profile, and Recovery Policy;
- Capability Catalog interface;
- deterministic syntax/semantic validation and policy-conflict detection;
- fee, route, finality, and recovery disclosure;
- institution authorization and credential boundary;
- Gateway API, endpoint, monitoring, alerting, receipt, reconciliation, incident, and upgrade coordination;
- public/basic layer versus paid enterprise layer;
- pilot partner, willingness to pay, and support economics;
- optional natural-language draft assistant.

Out of scope:

- direct LLM transaction execution;
- AI mutation of institution policy;
- raw KYC/PII on public chain;
- a single exclusive Hub enterprise operator or mandatory router;
- implementation of the route model or failover engine itself;
- final legal determination of a commercial SLA;
- any `automated regulatory compliance` claim;
- Gateway custody or discretionary execution of customer principal.

## 8. Local hard locks

- Preserve the sequence `Natural Language → Structured Intent → Validation → Disclosure → Confirmation`.
- Natural-language interpretation is a draft; structured fields are authoritative.
- Unsupported, ambiguous, or conflicting intent fails closed.
- Do not hide material route, fee, finality, or recovery risk behind abstraction.
- Preserve institution authorization and credential boundaries.
- The Gateway is a competitive operator product, not a Hub-exclusive customer interface.
- Keep institution policy text and PII off-chain/access-controlled.
- Capability and SLA references use factual CH-02 and CH-06 records.
- `One connection` never means one-provider monopoly.
- Paid value must be proven through integration, monitoring, reconciliation, and incident-cost reduction—not API calls alone.

## 9. Service classes, fields, and safe flow

Initial service classes remain Candidate:

`STANDARD`, `LOW-COST`, `FAST`, `RISK-ADJUSTED`, `ASSURED`, `INSTITUTIONAL`.

Minimum structured-intent fields:

```text
ASSET
AMOUNT
SOURCE
DESTINATION
MAX_TOTAL_COST
MINIMUM_RECEIVE
TARGET_COMPLETION
FINALITY_PROFILE
RELIABILITY_CLASS
ALLOWED_PROVIDER_POLICY
ALLOWED_PROTOCOL_POLICY
MAX_EXPOSURE
RECOVERY_POLICY
RECEIPT_PROFILE
AUTHORIZATION_REFERENCE
```

Safe processing flow:

```text
Optional Natural-language Draft
→ Structured Intent
→ Syntax / Semantic Validation
→ Policy Conflict Detection
→ Candidate Capability / Route / SLA Plans
→ Fee / Route / Finality / Recovery Disclosure
→ Institution Confirmation
→ Deterministic Transaction Construction
→ Cryptographic Verification
→ Execution
→ Institutional Receipt / Reconciliation
```

This is a Candidate sequence, not live authorization. AI/LLM cannot sign, approve, loosen policy, or execute.

## 10. Dependencies and outputs

Inputs:

- CH-02: SLO, finality, receipt, evidence completeness, recovery semantics;
- CH-04: route/failover/split capability and disclosure requirements;
- CH-06: factual provider/asset/capability catalog;
- CH-07: custody, agency, data, contract, support, and jurisdiction boundaries.

Outputs:

- To CH-01: enterprise distribution-interface requirements where needed.
- To CH-00: service classes, common intent objects, enterprise roadmap, and proposal-integration decisions.

Required artifacts:

1. `BM3-ENT-01` — ENTERPRISE_CUSTOMER_PROBLEM_AND_ACTOR_MAP
2. `BM3-ENT-02` — STRUCTURED_SERVICE_INTENT_SCHEMA
3. `BM3-ENT-03` — SERVICE_CLASS_AND_CAPABILITY_MAPPING
4. `BM3-ENT-04` — DETERMINISTIC_VALIDATION_DISCLOSURE_AUTHORIZATION_FLOW
5. `BM3-ENT-05` — ENTERPRISE_API_RECEIPT_RECONCILIATION_MODEL
6. `BM3-ENT-06` — PILOT_WTP_SUPPORT_ECONOMICS_GATE

## 11. Decision questions and gates

Questions:

- Which integration work does the institution need to eliminate?
- Which intent fields are mandatory or optional?
- How does each service class map to measurable capability?
- How do unsupported routes and conflicting intent fail closed?
- What fee/risk/finality/recovery information must be visible before approval?
- What is the public-Hub versus paid-operator boundary?
- How is protocol revenue attributed transparently from enterprise-operator revenue?

PASS only when structured intent rejects invalid/conflicting requests; material risk is disclosed and explicitly authorized; capability/SLA maps to factual evidence; integration/reconciliation/support reduction is measured; demand is paid or contractually credible; and operator competition/switching remain.

HOLD when interest exists but responsibility/data/support economics are unclear; correction/ambiguity remains high; or the catalog depends on marketing labels rather than evidence.

KILL/PIVOT when abstraction hides material risk; Gateway assumes custody or discretionary execution; no paid demand/protocol attribution exists; or direct LLM execution is required for the product to work.

Current start: close BM3-ENT-01 and BM3-ENT-02 before UI or LLM implementation discussion.

## 12. Validation, claims, handoff, and reporting

- Validate only changed claims, objects, and affected interfaces; no full re-research, global regression, or repeated validation loop.
- Separate fact, proposal, inference, and unverified hypothesis.
- Attach source class, implementation status, and claim ceiling where needed.
- Missing evidence is `UNKNOWN` or `HOLD`.
- Bind PASS to exact document/schema/data/code/contract scope.
- One optional-track failure does not invalidate unrelated tracks.
- Current maximum claim ceiling: `C2` before PoC.

CH-00 handoff fields: `FROM_CHANNEL`, `DECISION_ID`, `STATUS`, `QUESTION`, `RECOMMENDED_DECISION`, `ALTERNATIVES_CONSIDERED`, `EVIDENCE`, `RATIONALE`, `IMPACTED_CHANNELS`, `IMPACTED_BM`, `IMPACTED_TRACK`, `HARD_LOCK_CHECK`, `DEPENDENCIES`, `LEGAL_SAFETY_ECONOMIC_EFFECT`, `CLAIM_CEILING`, `OWNER_ACTION_REQUIRED`, `PROPOSED_INTEGRATION`, `SUPERSEDES`.

Channel reports use `OVERALL_PROGRESS`, `CURRENT_WORKSTREAM`, `CURRENT_QUESTION`, `CURRENT_BASELINE`, `MATERIAL_FINDINGS`, `DECISION_CANDIDATES`, `ALTERNATIVES`, `DEPENDENCIES`, `RISKS`, `BLOCKERS`, `OWNER_ACTION_REQUIRED`, and `NEXT_STEP`.
