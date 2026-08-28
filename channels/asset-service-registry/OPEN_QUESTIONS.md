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
