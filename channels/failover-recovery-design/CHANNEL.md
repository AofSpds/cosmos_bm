# CH-04 — FAILOVER RECOVERY DESIGN

## 1. Identity and exact source binding

- Project: `COSMOS HUB BM IMPROVEMENT`
- Target: `COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE`
- Channel ID: `CH-04`
- Canonical slug: `failover-recovery-design`
- Decision prefix: `BM2-MP-D`
- Role: BM2 Route Diversity / Failover / Split / Recovery Safety Channel
- Packet type: route diversity / failover / split / hedged separation / recovery safety / no live execution
- Effective packet date: `2026-08-29 KST`
- Exact charter source: `sources/raw/channel-policy-packets/v1.0/04_CH04_BM2_MULTIPATH_FAILOVER_RECOVERY_PACKET.md`
- Exact charter SHA-256: `1a5b466485fb19c44da66250c8399ad996a50ef08f2755c7e4e3b4a3d142b506`

This charter is derived from the corrected standalone packet above. The older archived E02 copy is not its authority.

## 2. Authority, decision effect, and authorization

Authority precedence:

1. Owner's latest explicit decision
2. Latest integrated decision from `CH-00 INTEGRATION / OWNER DECISIONS`
3. Common hard locks in this charter
4. Local hard locks and channel-sealed decisions
5. Working notes, hypotheses, and drafts

Decision lifecycle:

`WORKING → CANDIDATE → CHANNEL-SEALED → CH-00 REVIEWED → OWNER DECIDED → INTEGRATED`

- Channel conclusions are `CANDIDATE` by default and do not become project decisions before CH-00 integration and any required Owner choice.
- This channel does not silently alter another channel's scope, authority, or object definitions.
- A changed decision requires a new `BM2-MP-D` ID and explicit `SUPERSEDES`.
- `OWNER_ACTION_REQUIRED = FALSE` for bootstrap, investigation, and design discussion.
- `OWNER_ACTION_REQUIRED = TRUE` for an Owner selection, common-boundary change, proposal integration, pilot, implementation, or live test.
- Next Owner review: `BM2-MP-06`, when each mechanism needs its own Go/Hold/Kill choice.

Current authorization:

- Production: `NOT AUTHORIZED`
- Full v1.2 rewrite: `NOT AUTHORIZED`
- New/fifth BM: `NOT AUTHORIZED`
- Native module design: `NOT AUTHORIZED`
- Live routing or financial execution: `NOT AUTHORIZED`
- Commercial SLA or compensation: `NOT AUTHORIZED`
- Formal 6G conformity claim: `NOT AUTHORIZED`

v1.1 is an independent proposal `CANDIDATE`, not official Hub policy. STEP 3–5 is an `OWNER-REVIEW CANDIDATE`. The portfolio is `B. SELECTIVE FIT — CANDIDATE`. `OR-01` through `OR-09` remain `UNDECIDED`.

## 3. Locked four-BM order

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

## 4. Common hard locks

- Preserve `Thin Core, Rich Edges`.
- Base IBC remains open; no forced Hub toll on base IBC.
- The Hub does not custody customer principal.
- ATOM is not a mandatory payment asset.
- Do not add a Hub-owned DEX, bridge, lending market, perpetuals venue, stablecoin, market maker, or proprietary mandatory router.
- Do not place raw KYC/PII or an institution's sensitive policy text on public chain.
- Validate contracts and data, then a small audited CosmWasm MVP, before any native module.
- A native module requires a proven repeated-operational bottleneck and separate Owner approval.
- AI does not hold private keys, authorize transactions, mutate hard policy/exposure/minimum receive/finality/allowlists, or decide compensation/legal responsibility unilaterally.
- Do not imply global atomic revert, principal guarantee/protection, insurance, or regulatory suitability/compliance.
- Preserve open provider competition, public specifications, switching, and no exclusive mandatory operator.
- Do not claim `6G-compliant`, `6G-certified`, `IMT-2030 compliant`, or `3GPP 6G implemented`.
- The roadmap is selective prior-art adaptation, not a production architecture approval.

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

## 6. Mission and mandatory mechanism separation

Primary question: which of Candidate Route Diversity, Sequential Failover, Split Routing, and Redundant/Hedged Execution actually improves reliability and economics, and where should each stop independently?

Mission: never collapse the four mechanisms into a generic `multi-path` feature. Evaluate each mechanism's state machine, duplicate safety, asset location, recovery, and net value separately.

Mandatory classification and current baseline:

| Mechanism | Meaning | Current source-derived status |
|---|---|---|
| A. Candidate Route Diversity | Compute several routes and choose one | `EXISTING / PARTIAL`; roadmap baseline, not a new claim |
| B. Sequential Failover | Switch to another route before execution or at an explicit safe point | `PARTIAL / SELECT-LIMITED`; start with pre-execution replacement |
| C. Split Routing | Divide value among legs to optimize output/capacity | Smart-Swap is `EXISTING / PARTIAL`; broader use needs separate evidence |
| D. Redundant / Hedged Execution | Execute multiple routes concurrently to reduce tail/failure risk | `WATCH / DEFAULT-OFF`; high-risk independent track |

All dispositions are Candidate. Sequential failover is not a global mid-flight reroute, global atomic-revert mechanism, principal guarantee, or live authorization.

## 7. Scope

In scope:

- candidate route set and route-plan hash;
- pre-execution health checks, quote expiry, and route replacement;
- failover point before and after authorization;
- idempotency, bounded retry, unique execution ID, and duplicate suppression;
- per-leg amount and exposure cap;
- leg state and aggregate-completion rule;
- last-known asset location;
- partial completion and stranded intermediate assets;
- recovery owner, deadline, and capital release;
- provider fee, gas, liquidity, recovery, support, locked-capital, compliance, and accounting cost;
- independent PASS/HOLD/KILL for diversity, failover, split, and hedge;
- historical replay and bounded failure simulation.

Out of scope:

- AI model training or prediction-performance work;
- final definition of SLO or legal breach;
- provider eligibility or Registry badges;
- enterprise service UX;
- production multi-path deployment;
- generic automatic-recovery or global-atomicity claims.

## 8. Local hard locks and invariants

Local hard locks:

- Never merge the four mechanisms into one feature or KPI.
- Hedged Execution is `DEFAULT-OFF` and has no live test without separate Owner approval.
- Do not reroute when the exact failover point or current asset location is unclear.
- Do not advance without a unique execution ID and duplicate suppression.
- Every split/hedge leg needs an independent receipt and recovery owner.
- Freeze the aggregate-completion rule before execution.
- Net value subtracts additional cost, locked capital, and recovery; success benefit alone is insufficient.
- Do not relabel current Smart-Swap capability as a new Cosmos Hub function.
- An AI health score is an input signal, not execution permission.
- Mid-flight failover requires a materially higher Safety Gate than pre-execution replacement.

Mandatory invariants:

```text
unique execution ID
route-plan hash
per-leg amount and exposure cap
leg start / complete / fail state
aggregate completion rule
last-known asset location
duplicate suppression
recovery owner and deadline
capital-release rule
compensation reference
```

Net Route Value:

```text
Incremental Success / Output / Tail-Latency Benefit
- Extra Provider Fee
- Extra Gas
- Liquidity / Price Impact
- Recovery and Support Cost
- Locked-Capital Cost
- Compliance / Accounting Overhead
= Net Route Value
```

## 9. Ordered evaluation

1. Record existing candidate route diversity as the baseline.
2. Add pre-execution provider/client/channel health checks.
3. Evaluate deterministic route replacement before authorization.
4. Evaluate bounded retry only where idempotency is proven.
5. Evaluate split only with per-leg receipts.
6. Keep Hedged Execution as a separate research track.

Do not start implementation discussion before BM2-MP-02 through BM2-MP-04 define the state, idempotency, location, and recovery model.

## 10. Dependencies and outputs

Inputs:

- CH-02: time, leg, failure, recovery, last-known-location evidence semantics;
- CH-03: advisory route-risk/health estimates and confidence;
- CH-06: provider capability, route support, and incident history;
- CH-07: duplicate liability, partial-leg accounting, exposure, and compensation boundary.

Outputs:

- To CH-05: user/institution disclosure requirements for route, failover, split, and recovery.
- To CH-00: an independent promotion/kill decision for each mechanism.

Required artifacts:

1. `BM2-MP-01` — MULTIPATH_TAXONOMY_AND_EXISTING_BASELINE
2. `BM2-MP-02` — ROUTE_PLAN_LEG_AND_STATE_MACHINE
3. `BM2-MP-03` — IDEMPOTENCY_DUPLICATE_SUPPRESSION_INVARIANTS
4. `BM2-MP-04` — RECOVERY_ASSET_LOCATION_AND_CAPITAL_RELEASE_MODEL
5. `BM2-MP-05` — NET_ROUTE_VALUE_ASSESSMENT
6. `BM2-MP-06` — INDEPENDENT_GO_HOLD_KILL_DECISIONS

## 11. PASS / HOLD / KILL

Route diversity PASS: trust, liquidity, and health differences among candidate routes can be compared factually.

Sequential failover PASS only when the failover point is exact; duplicate execution is prevented; quote, minimum receive, and policy are revalidated; asset location and recovery are reproducible; and net value is positive.

Split PASS only when per-leg evidence and aggregate completion are exact, partial-failure recovery is feasible, and realized-output benefit exceeds added cost.

Hedge has no default PASS. It may return as a Candidate only after duplicate-settlement prevention, accounting/legal treatment, capital release, and net value are separately proven.

HOLD when benefit is narrow; per-leg evidence/idempotency is incomplete; or asset location/recovery owner is unclear.

KILL when duplicate execution or stranded assets remain; recovery/accounting worsens; net value is negative; or safety requires global custody or exclusive Hub execution.

## 12. Validation, claims, handoff, and reporting

- Validate only changed claims, objects, and affected interfaces.
- No full re-research, global regression, or repeated validation loop.
- Separate facts, proposals, inferences, and unverified hypotheses.
- Attach source class, implementation status, and claim ceiling where needed.
- Missing evidence means `UNKNOWN` or `HOLD`, not inference.
- Bind PASS to exact document/schema/data/code/contract scope.
- A failed optional mechanism does not invalidate unrelated tracks.
- Current claim ceiling: `C2` before PoC.

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

Channel reports use `OVERALL_PROGRESS`, `CURRENT_WORKSTREAM`, `CURRENT_QUESTION`, `CURRENT_BASELINE`, `MATERIAL_FINDINGS`, `DECISION_CANDIDATES`, `ALTERNATIVES`, `DEPENDENCIES`, `RISKS`, `BLOCKERS`, `OWNER_ACTION_REQUIRED`, and `NEXT_STEP`.
