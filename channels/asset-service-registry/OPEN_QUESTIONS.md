# CH-06 Open Questions

All recommendations remain Candidate; no Owner choice is inferred.

## Owner review sheet — all undecided

| ID | Open decision | Candidate recommendation | State |
|---|---|---|---|
| OR-01 | Accept `B. SELECTIVE FIT`? | Yes | `UNDECIDED` |
| OR-02 | Approve SELECT concepts, including capability exposure? | Yes | `UNDECIDED` |
| OR-03 | Approve SELECT-LIMITED conflict arbitration? | Yes behind gates | `UNDECIDED` |
| OR-04 | Treat Route Diversity/Split as existing? | Yes | `UNDECIDED` |
| OR-05 | Keep replay/agentic/hedged as WATCH? | Yes | `UNDECIDED` |
| OR-06 | Reject zero-touch/slicing/RAN/Hub router? | Yes | `UNDECIDED` |
| OR-07 | Approve roadmap as Candidate? | Yes as Candidate only | `UNDECIDED` |
| OR-08 | Prefer Main Text + Annex later? | Preliminary yes | `UNDECIDED` |
| OR-09 | Keep C2 pre-PoC ceiling? | Yes | `UNDECIDED` |

## BM4-REG-01 — Asset Record and issuer declaration

- What is the minimum public factual Asset Record?
- How are issuer-declared canonical representation, signature, reserve/document/attestation pointers, and external verification distinguished?
- How are version, freshness, revocation, and conflicts represented without a `safe` or `approved` implication?

Closure: versioned schema and signed examples separating declaration, pointer, and verification status.

## BM4-REG-02 — Provider and Capability Record

- Which minimum fields are mandatory for each service type?
- How are supported assets/routes/protocols, quote interface, capability signature, jurisdiction/policy reference, and evidence sources represented?
- Which details remain off-chain due to PII, policy, telemetry, or trade-secret boundaries?

Closure: versioned factual schema with public/off-chain classification.

## BM4-REG-03 — freshness, incidents, and revocation

- What makes evidence fresh, stale, missing, disputed, or revoked?
- How are incident scope, source, resolution state, and subsequent remediation recorded?
- Which sources independently corroborate self-reported telemetry?

Closure: deterministic freshness/revocation rules, incident lifecycle, and evidence-source hierarchy.

## BM4-REG-04 — eligibility, ranking, and confidence

- Which rules are deterministic eligibility and which outputs are model ranking/opinion?
- How are confidence intervals, missingness, model/version, and abstention disclosed?
- How is low score prevented from automatic expulsion and high score from becoming an approval badge?

Closure: separate schemas/flows and adversarial tests for bias, gaming, concentration, and stale data.

## BM4-REG-05 — open entry, switching, and concentration

- What newcomer evaluation path prevents permanent exclusion from limited history?
- How are switching friction, top-provider share, and concentration trend measured?
- How does the design avoid mandatory routing, exclusive operators, or proprietary-data advantage?

Closure: open-entry/switching policy, concentration metrics/alerts, and operator-neutral interfaces.

## BM4-REG-06 — conflict detection and arbitration

- How are conflicting asset representations, capability statements, quotes, revocations, and policy references detected?
- What published deterministic priority rules apply, and who may pause/review a dispute?
- How is every input and outcome auditably linked without a hidden super-agent decision?

Closure: signed-input conflict taxonomy, deterministic resolution table, audit trail, and unresolved-state treatment.

## Current action boundary

Proceed with factual schemas BM4-REG-01 through BM4-REG-03. Do not issue badges, choose providers, publish sensitive data, build a mandatory router, start production, or replace legal certification.

## Tagged Owner-question and decision-point continuity register — 2026-08-29 KST

Full wording, intuitive explanation, hardcore scope, dependencies, and tags are maintained in `TOPIC_INDEX.md`. All entries below are `OPEN / UNDECIDED` unless an explicit later Owner answer is recorded.

| Range | Subject |
|---|---|
| `BM4-OQ-001` | Registry operator/governance model |
| `BM4-OQ-002`–`005` | Asset Record, issuer authority, attestation and representation conflict |
| `BM4-OQ-006`–`008` | Provider identity, open/pseudonymous entry and signer rotation |
| `BM4-OQ-009`–`012` | Capability mandatory fields, limits, bond reference and BM3 service mapping |
| `BM4-OQ-013`–`014` | Signed Quote publication, privacy and retention |
| `BM4-OQ-015`–`017` | Evidence-source hierarchy, corroboration and retention |
| `BM4-OQ-018`–`019` | Freshness windows and stale-data eligibility effect |
| `BM4-OQ-020`–`022` | Incident severity, disclosure and review authority |
| `BM4-OQ-023`–`025` | Revocation, appeal, reinstatement and cascade |
| `BM4-OQ-026`–`028` | Deterministic eligibility and UNKNOWN treatment |
| `BM4-OQ-029`–`031` | Ranking surface, metrics, model audit and abstention |
| `BM4-OQ-032`–`034` | Newcomer evaluation, exposure caps and anti-sybil balance |
| `BM4-OQ-035`–`036` | Switching, portability and friction KPI |
| `BM4-OQ-037`–`038` | Concentration metrics, thresholds and response |
| `BM4-OQ-039`–`040` | Conflict detection effects and disclosure boundary |
| `BM4-OQ-041`–`043` | Arbitration priority, unresolved state and review/appeal |
| `BM4-OQ-044`–`045` | Public/on-chain minimum and privacy/linkability risk |
| `BM4-OQ-046`–`047` | Query, ranking UX, public API and paid feed |
| `BM4-OQ-048`–`049` | Security, anti-sybil, false capability and telemetry sanctions |
| `BM4-OQ-050`–`051` | Registry liability, reliance and third-party attestation |
| `BM4-OQ-052`–`054` | Fees, revenue, free/public boundary and newcomer barrier |
| `BM4-OQ-055`–`056` | Schema/rule governance and emergency change |
| `BM4-OQ-057` | CH-00 shared-object promotion order |
| `BM4-OQ-058`–`060` | Bounded MVP universe, content and operator/evidence candidates |
| `BM4-OQ-061` | KPI thresholds for BM4-REG-01 through 06 closure |

Pending decision points are `BM4-DP-001` through `BM4-DP-025`. They cover operating model; Asset/Provider/Capability/Quote schemas; evidence/freshness/incident/revocation; eligibility/ranking; open entry/switching/concentration; conflict/arbitration; data placement; API/UX; security; legal; economics; governance; shared objects; MVP; and promotion KPIs.

A `BM4-DP` tag is a decision point only. It must not be represented as `OWNER_DECIDED`, `CHANNEL-SEALED`, or `INTEGRATED` until the corresponding explicit authority and Git records exist.
