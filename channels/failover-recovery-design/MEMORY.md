# CH-04 Current Memory

`MEMORY_TYPE = COMPRESSED CURRENT STATE / NOT A TRANSCRIPT`

## Identity and authority

- Channel: `CH-04 FAILOVER RECOVERY DESIGN`
- Slug: `failover-recovery-design`
- Decision prefix: `BM2-MP-D`
- Corrected charter: `sources/raw/channel-policy-packets/v1.0/04_CH04_BM2_MULTIPATH_FAILOVER_RECOVERY_PACKET.md`
- Charter SHA-256: `1a5b466485fb19c44da66250c8399ad996a50ef08f2755c7e4e3b4a3d142b506`
- Authority: latest Owner decision → CH-00 integration → common hard locks → local/channel-sealed decision → working material.
- This memory is context, not authority.

## Programme state

- v1.1: `CANDIDATE / INDEPENDENT / NOT OFFICIAL HUB POLICY`
- STEP 3–5: `OWNER-REVIEW CANDIDATE`
- Overall: `B. SELECTIVE FIT — CANDIDATE`
- OR-01–OR-09: `UNDECIDED / DO NOT AUTO-INFER`
- Production, full v1.2 rewrite, fifth BM, native module, live routing/financial execution, commercial SLA/compensation, and formal 6G conformity: `NOT AUTHORIZED`
- Claim ceiling: `C2 BEFORE POC`

## Locked BM order and common boundaries

1. Interchain Asset Distribution Market
2. Assured Interchain Delivery SLA
3. Enterprise One-Connection Gateway
4. Asset & Service Registry

- Thin Core, Rich Edges; open base IBC; no forced Hub toll.
- No Hub customer-principal custody; no mandatory ATOM payment.
- No Hub-owned DEX, bridge, lending, perp, stablecoin, market making, or mandatory proprietary router.
- No public-chain raw KYC/PII or sensitive institution policy.
- Contract/data and small audited CosmWasm before any separately approved native module.
- No AI key custody, transaction authorization, hard-policy/exposure/minimum-receive/finality/allowlist mutation, or unilateral compensation/legal decision.
- No global atomic revert, principal guarantee/protection, insurance, or compliance implication.
- Preserve provider competition, public specification, switching, and no exclusive operator.
- No 6G compliance/certification/implementation claim; roadmap is not production approval.

## Current mechanism state — all source-derived Candidate

- Candidate Route Diversity: `EXISTING / PARTIAL`; baseline, not new.
- Sequential Failover: `PARTIAL / SELECT-LIMITED`; begin with pre-execution health check and deterministic replacement.
- Smart-Swap Split Routing: `EXISTING / PARTIAL`; broader cross-protocol use is not baseline.
- Redundant/Hedged Execution: `WATCH / DEFAULT-OFF`; no live test or default PASS.

Sequential failover does not mean arbitrary mid-flight rerouting, global atomic revert, or principal guarantee.

## Required invariant state

No implementation discussion advances without unique execution ID, route-plan hash, per-leg amount/exposure cap, leg states, aggregate-completion rule, last-known asset location, duplicate suppression, recovery owner/deadline, capital release, and compensation reference.

The evaluation order is baseline diversity → pre-execution health → pre-authorization replacement → idempotent bounded retry → per-leg split evaluation → independent hedge research.

## Current work

- Start at `BM2-MP-01`, freezing existing/partial/new classification.
- Then close `BM2-MP-02` state machine, `BM2-MP-03` idempotency, and `BM2-MP-04` recovery/location before implementation discussion.
- `BM2-MP-05` measures net route value after every incremental cost.
- `BM2-MP-06` asks for independent Go/Hold/Kill per mechanism and is the next Owner-review point.
- No channel-sealed, CH-00-reviewed, Owner-decided, or integrated BM2-MP decision exists at bootstrap.

## Dependencies

- CH-02 supplies evidence semantics; CH-03 advisory risk/health; CH-06 capability/history; CH-07 liability/accounting/exposure.
- CH-05 receives disclosure requirements; CH-00 receives independent mechanism decisions.

## Owner-directed conversation and response protocol — 2026-08-29 KST

This is an `OWNER_EXPLICIT_OPERATIONAL_DIRECTION`, not a BM semantic decision and not a mechanism PASS.

- Every substantive CH-04 answer explains the active item first in plain language, then in technical/hardcore depth.
- Owner questions and Owner decision points are visibly tagged and kept separate from design questions, source gaps, Candidate recommendations and hard locks.
- Every substantive answer ends with a compact `[CH-04 TOPIC TRACKER]` covering the stable topic IDs below, current status, Owner tags and next exact item.
- A topic is not marked complete merely because it was discussed. Completion requires the closure evidence defined for its BM2-MP deliverable.
- Material changes are summarized in the channel checkpoint. Git persistence remains branch-bounded and does not imply Owner acceptance or integration.

### Stable topic IDs

```text
MP-00  Authority, scope and claim boundary
MP-01  Four-mechanism taxonomy and existing baseline
MP-02  Route universe, comparability and independence
MP-03  Request, quote, route-plan and leg objects
MP-04  Route/leg/recovery state machine
MP-05  Exact failover points and authorization boundary
MP-06  Idempotency, replay and duplicate suppression
MP-07  Per-leg amount, exposure and aggregate completion
MP-08  Last-known asset location and asset lineage
MP-09  Recovery actions, owner, deadline and terminal states
MP-10  Capital lock, release, bond and compensation references
MP-11  Evidence, timestamps, finality and source corroboration
MP-12  Failure taxonomy and controllability classification
MP-13  Quote/policy/finality/recovery revalidation
MP-14  Split-routing partial completion and accounting
MP-15  Hedged-execution safety and default-off test
MP-16  Net Route Value and mechanism-specific economics
MP-17  Provider neutrality and architecture placement
MP-18  Legal, accounting, liability and disclosure interfaces
MP-19  Replay, simulation, adversarial and PoC test design
MP-20  Per-mechanism Go/Hold/Kill and CH-00 handoff
MP-21  Cross-channel dependencies and interface contracts
MP-22  Claim language and communication ceiling
MP-23  BM2-MP-01 through BM2-MP-06 progress and memory maintenance
```

## Succession rule

- Validate only changed claims/objects/interfaces; missing evidence is `UNKNOWN` or `HOLD`.
- `DECISIONS.jsonl` is append-only and source-derived at bootstrap.
- `HANDOFF_CURRENT.md` mirrors memory and decisions only; regenerate after material change.
