# CH-05 Open Questions

All recommendations remain Candidate; no Owner choice is inferred.

## Owner review sheet — all undecided

| ID | Open decision | Candidate recommendation | State |
|---|---|---|---|
| OR-01 | Accept `B. SELECTIVE FIT`? | Yes | `UNDECIDED` |
| OR-02 | Approve SELECT concepts, including structured intent? | Yes | `UNDECIDED` |
| OR-03 | Approve SELECT-LIMITED items, including draft-only NL assistant? | Yes behind gates | `UNDECIDED` |
| OR-04 | Treat Route Diversity/Split as existing? | Yes | `UNDECIDED` |
| OR-05 | Keep replay/agentic/hedged as WATCH? | Yes | `UNDECIDED` |
| OR-06 | Reject zero-touch/slicing/RAN/Hub router? | Yes | `UNDECIDED` |
| OR-07 | Approve the roadmap as Candidate? | Yes as Candidate only | `UNDECIDED` |
| OR-08 | Prefer Main Text + Annex later? | Preliminary yes | `UNDECIDED` |
| OR-09 | Keep C2 pre-PoC ceiling? | Yes | `UNDECIDED` |

## BM3-ENT-01 — customer problem and actors

- Which exact integration, monitoring, reconciliation, incident, and upgrade work is reduced?
- Who is the customer, Gateway operator, provider, wallet/custodian, evidence operator, and contract party?
- Which work belongs to the public/basic layer versus a paid competitive operator?

Closure: actor/problem map, current integration baseline, measurable cost/time burden, and credible customer evidence.

## BM3-ENT-02 — structured intent schema

- Are all minimum fields necessary, and which additional fields are optional?
- How are unsupported, ambiguous, missing, and conflicting fields represented and failed closed?
- How are policy profiles, route constraints, finality, exposure, recovery, receipt, and authorization references versioned?

Closure: versioned schema, field semantics, validation rules, invalid examples, and authority boundary.

## BM3-ENT-03 — service-class mapping

- How do STANDARD, LOW-COST, FAST, RISK-ADJUSTED, ASSURED, and INSTITUTIONAL map to measurable CH-02/CH-06 facts?
- How are stale/missing capability records disclosed instead of turned into marketing labels?
- How does switching work across Gateway operators and providers?

Closure: factual service-class/capability matrix with no approved/safe/compliant implication.

## BM3-ENT-04 — validation, disclosure, and authorization

- Which conflicts must stop processing?
- What fee, route, trust, finality, partial-completion, and recovery risks must the institution see before confirmation?
- How is credential and authorization scope separated from natural-language drafting and candidate planning?

Closure: deterministic flow, fail-closed tests, disclosure receipt, and explicit institution-authorization proof.

## BM3-ENT-05 — API, receipt, and reconciliation

- What endpoint, monitoring, alert, evidence, receipt, accounting, and incident formats are required?
- Which fields remain off-chain/access-controlled, and which minimum references may be public?
- How are source/destination/leg/recovery records reconciled when sources disagree?

Closure: API/receipt/reconciliation Candidate with privacy and evidence provenance.

## BM3-ENT-06 — pilot, WTP, and support economics

- Is demand paid or contractually credible?
- What integration savings, support load, incident cost, liability, renewal, and protocol-share attribution are expected?
- Can the product work without custody, discretionary execution, direct LLM execution, monopoly, or hidden material risk?

Closure: bounded pilot proposal and economics evidence. Owner approval remains separately required.

## Current action boundary

Proceed with BM3-ENT-01 and BM3-ENT-02 design. Do not build UI/LLM execution, select an operator, start a pilot, publish KYC/PII, promise a commercial SLA, or rewrite the proposal.
