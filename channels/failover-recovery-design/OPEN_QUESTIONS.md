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

## CH-04 tagging vocabulary

| Tag | Meaning |
|---|---|
| `[OWNER-LOCKED]` | already fixed by an explicit Owner/common hard lock; do not reopen by inference |
| `[OWNER-DIR-PROCESS]` | Owner's operating instruction for this channel; not a BM semantic decision |
| `[OWNER-Q-LATER]` | prepare alternatives and evidence now; ask the Owner only at the named gate |
| `[OWNER-DECISION-PENDING]` | channel cannot finalize the item; explicit Owner choice is eventually required |
| `[DESIGN-Q]` | BM_MASTER may develop a Candidate answer without current Owner action |
| `[SOURCE-Q]` | requires exact implementation or source evidence before a design conclusion |
| `[CH-00-REVIEW]` | shared object/interface or project-level promotion requires CH-00 integration |
| `[NO-OWNER-ACTION-NOW]` | bounded analysis may proceed without interrupting the Owner |

## Tagged question and decision register

| ID | Related topic | Tag | Question or decision | Earliest escalation point | Current state |
|---|---|---|---|---|---|
| `OQ-MP-01` | MP-01/02 | `[SOURCE-Q] [DESIGN-Q]` | What route-diversity and split behavior exists today, and what route universe is factually comparable? | BM2-MP-01 closure | OPEN / no Owner action now |
| `OQ-MP-02` | MP-04/05 | `[DESIGN-Q]` | Which exact state transitions remain replaceable, authorized-but-unbroadcast, committed, or recovery-only? | BM2-MP-02 closure | OPEN / no Owner action now |
| `OQ-MP-03` | MP-05 | `[OWNER-Q-LATER] [OWNER-DECISION-PENDING]` | After Candidate evidence is complete, should Sequential Failover stop permanently at pre-execution replacement, or may a separately gated post-authorization retry scope be retained? | BM2-MP-06; earlier only if scope expansion is requested | UNDECIDED |
| `OQ-MP-04` | MP-06 | `[DESIGN-Q] [SOURCE-Q]` | Which provider/protocol operations can prove idempotency, at-most-once effect, or safe retry under delayed acknowledgements? | BM2-MP-03 closure | OPEN / no Owner action now |
| `OQ-MP-05` | MP-08/09 | `[DESIGN-Q] [OWNER-Q-LATER]` | Which actor is recovery owner for each terminal/non-terminal state, and where must responsibility transfer be explicit? | Candidate recommendation at BM2-MP-04; Owner choice at BM2-MP-06 if commercial responsibility changes | OPEN |
| `OQ-MP-06` | MP-10/18 | `[OWNER-Q-LATER] [CH-00-REVIEW]` | What capital-release deadline, reserve/bond reference, and compensation boundary is acceptable without creating a principal guarantee or unbounded liability? | After CH-07 input; before any commercial pilot | UNDECIDED |
| `OQ-MP-07` | MP-07/14 | `[OWNER-Q-LATER] [OWNER-DECISION-PENDING]` | For Split Routing, should aggregate completion require all legs, a minimum realized amount, or an explicitly bounded partial-completion class? | BM2-MP-06 after technical/accounting alternatives are complete | UNDECIDED |
| `OQ-MP-08` | MP-15/20 | `[OWNER-DECISION-PENDING]` | Should Hedged Execution remain WATCH, move to permanent HOLD, or be KILLed after the evidence package? | BM2-MP-06 | UNDECIDED / default-off |
| `OQ-MP-09` | MP-16 | `[DESIGN-Q] [OWNER-Q-LATER]` | What minimum positive Net Route Value and confidence level justify promotion for each mechanism? | Threshold recommendation in BM2-MP-05; Owner decision in BM2-MP-06 | OPEN |
| `OQ-MP-10` | MP-19 | `[OWNER-DECISION-PENDING]` | What exact asset/chain/provider/exposure universe, if any, may enter a later bounded PoC? | Separate pilot authorization after BM2-MP-06 | NOT AUTHORIZED |
| `OQ-MP-11` | MP-21 | `[CH-00-REVIEW]` | Which shared fields are owned by CH-02 evidence, CH-05 intent, CH-06 registry, and CH-07 legal/economics rather than CH-04? | Interface-contract handoff | OPEN |
| `OQ-MP-12` | MP-00/22 | `[OWNER-LOCKED]` | May this channel claim generic multi-path reliability, live failover, principal protection, or global atomicity? | No escalation; answer remains NO unless the Owner explicitly supersedes the hard locks | CLOSED / prohibited |
| `OQ-MP-13` | MP-23 | `[OWNER-DIR-PROCESS]` | How should answers and memory be maintained? | Effective immediately | DECIDED FOR PROCESS: plain-language first, hardcore second, tracker appended |

## Current action boundary

Bounded taxonomy/state/recovery design may continue. No implementation, pilot, live test, hedged execution, commercial commitment, or global guarantee language is authorized.
