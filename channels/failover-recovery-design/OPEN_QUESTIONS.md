# CH-04 Open Questions

Recommendations below remain Candidate. No Owner choice is inferred.

## Owner review sheet — all undecided

| ID | Open decision | Candidate recommendation | State |
|---|---|---|---|
| OR-01 | Accept `B. SELECTIVE FIT`? | Yes | `UNDECIDED` |
| OR-02 | Approve SELECT concepts? | Yes | `UNDECIDED` |
| OR-03 | Approve SELECT-LIMITED items behind gates? | Yes; includes Sequential Failover | `UNDECIDED` |
| OR-04 | Treat Route Diversity/Split as existing? | Yes | `UNDECIDED` |
| OR-05 | Keep replay/agentic/hedged as WATCH? | Yes | `UNDECIDED` |
| OR-06 | Reject zero-touch/slicing/RAN/Hub router? | Yes | `UNDECIDED` |
| OR-07 | Approve roadmap as Candidate? | Yes as Candidate only | `UNDECIDED` |
| OR-08 | Preliminary Option B preference? | Yes, subject to STEP 9 | `UNDECIDED` |
| OR-09 | Keep C2 pre-PoC ceiling? | Yes | `UNDECIDED` |

## BM2-MP-01 — taxonomy and baseline

- Which current route-diversity and Smart-Swap split functions are directly evidenced, and where does each stop?
- Which retry, refund, or status functions are protocol-specific rather than general sequential failover?
- What exact route universe is comparable without mislabeling an existing provider function as a new Hub capability?

Closure: exact implementation/source mapping and existing/partial/new matrix.

## BM2-MP-02 — route/leg state machine

- What is the exact failover point before and after authorization?
- Which state transition commits a leg, and which states still permit deterministic replacement?
- How are quote expiry, minimum receive, finality, policy, and route-plan hash revalidated?
- How is aggregate completion defined before execution?

Closure: versioned route-plan and leg state machine with invalid transitions.

## BM2-MP-03 — idempotency and duplicate suppression

- How is a unique execution ID propagated across providers and protocols?
- Which retry scopes are provably idempotent?
- What prevents duplicate settlement across route replacement, split legs, or delayed acknowledgements?

Closure: duplicate-suppression invariant, idempotency proof scope, and replay/adversarial cases.

## BM2-MP-04 — recovery and asset location

- Can last-known asset location be reconstructed for every partial-failure state?
- Who owns recovery, by what deadline, and when is locked capital released?
- What receipt and compensation reference attaches to each leg?

Closure: reproducible location/recovery/capital-release model for every simulated failure state.

## BM2-MP-05 — net route value

- Does added success, output, or tail-latency benefit exceed provider fee, gas, liquidity impact, recovery/support, locked capital, and compliance/accounting cost?
- For which route segments is benefit positive, narrow, or negative?

Closure: bounded measured comparison against deterministic existing baselines.

## BM2-MP-06 — independent mechanism choices

Owner choice will be required only after separate evidence packages exist for Route Diversity, Sequential Failover, Split, and Hedge. A failure in one mechanism must not invalidate unrelated mechanisms.

## Current action boundary

Bounded taxonomy/state/recovery design may continue. No implementation, pilot, live test, hedged execution, commercial commitment, or global guarantee language is authorized.
