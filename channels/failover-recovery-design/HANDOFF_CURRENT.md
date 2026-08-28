# CH-04 Current Handoff

`ARTIFACT_CLASS = DERIVED CONTEXT ONLY / NO INDEPENDENT AUTHORITY`

Regenerate from current Git, `MEMORY.md`, `DECISIONS.jsonl`, and `OPEN_QUESTIONS.md` after a material change. Higher-authority Owner, CH-00, and charter records prevail.

GENERATION_STAGE = `OWNER_DIRECTED_CHANNEL_TOPIC_CURRENTIZATION_CANDIDATE`
CURRENTIZATION_CLASS = `CHANNEL MEMORY MAINTENANCE / RESPONSE PROTOCOL`
TASK_ID = `COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829`
BASE_MAIN_SHA = `562850c0639cdf04462f9520166be1e6f9880aab`
CANDIDATE_BRANCH = `bm-master/ch04-topic-map-response-protocol-20260829`
DERIVED_INPUTS = `MEMORY.md + DECISIONS.jsonl + OPEN_QUESTIONS.md`

FROM_CHANNEL = `CH-04 — FAILOVER RECOVERY DESIGN`
DECISION_ID = `BM2-MP-D-0001`
STATUS = `CANDIDATE / NOT CHANNEL-SEALED / NO OWNER BM DECISION`
QUESTION = How should route diversity, sequential failover, split routing, and hedged execution remain separately defined and evaluated?
RECOMMENDED_DECISION = Keep the four mechanisms distinct; evaluate sequential failover as pre-execution-first and keep hedged execution WATCH/default-off.
ALTERNATIVES_CONSIDERED = Generic multi-path reliability, live hedge activation, global atomic revert, and principal protection; excluded by evidence and hard-lock boundaries.
EVIDENCE = Exact CH-04 packet SHA-256 `1a5b466485fb19c44da66250c8399ad996a50ef08f2755c7e4e3b4a3d142b506`; current source hashes in `SOURCES.md`.
RATIONALE = The mechanisms have different capital, duplicate-execution, recovery, and observability risks and cannot share an undifferentiated reliability claim.
IMPACTED_CHANNELS = CH-02 evidence, CH-03 prediction, CH-05 disclosure, CH-06 provider facts, CH-07 responsibility/economics, CH-00 promotion
IMPACTED_BM = BM2 directly; supporting interfaces for BM3 and BM4
IMPACTED_TRACK = Pre-PoC mechanism taxonomy, state machine, recovery, and net-value evidence
HARD_LOCK_CHECK = Preserved; no live authority, global atomic revert, principal guarantee, insurance, custody, or proprietary mandatory router
DEPENDENCIES = CH-02 event/finality/recovery semantics; route and leg state; idempotency; provider evidence; legal responsibility and exposure bounds
LEGAL_SAFETY_ECONOMIC_EFFECT = None authorized; compensation, reserve, recovery liability, and commercial commitment remain unresolved
CLAIM_CEILING = `C2 — pre-PoC maximum`
OWNER_ACTION_REQUIRED = `FALSE` now; `TRUE` only when a bounded Go/Hold/Kill or pilot choice is ready
PROPOSED_INTEGRATION = None until `BM2-MP-01`–`06` close and a channel-sealed handoff is submitted
SUPERSEDES = None

## Identity and read order

- Channel: `CH-04 FAILOVER RECOVERY DESIGN`
- Slug / prefix: `failover-recovery-design` / `BM2-MP-D`
- Charter: `sources/raw/channel-policy-packets/v1.0/04_CH04_BM2_MULTIPATH_FAILOVER_RECOVERY_PACKET.md`
- SHA-256: `1a5b466485fb19c44da66250c8399ad996a50ef08f2755c7e4e3b4a3d142b506`
- Read: current Git/governance → `CHANNEL.md` → `MEMORY.md` → `DECISIONS.jsonl` → `OPEN_QUESTIONS.md` → `SOURCES.md` → `WORKLOG.md` → this handoff.

## Current state reproduced

- v1.1: Candidate, independent, not official Hub policy.
- STEP 3–5: Owner-review Candidate.
- Overall: `B. SELECTIVE FIT — CANDIDATE`; OR-01–OR-09 all `UNDECIDED`.
- Claim ceiling: C2 before PoC.
- Production, rewrite, fifth BM, native module, live routing/financial execution, commercial SLA/compensation, and formal 6G conformity are not authorized.

Locked BM order: Distribution Market → Assured Delivery SLA → Enterprise Gateway → Asset & Service Registry.

Hard locks: Thin Core/Rich Edges; open untolled base IBC; no Hub customer-principal custody or mandatory ATOM; no Hub DEX/bridge/lending/perp/stablecoin/market-making/proprietary mandatory router; no raw KYC/PII or sensitive policy on public chain; contract/data and small audited CosmWasm first; no AI keys, authorization, hard-policy mutation, or unilateral compensation; no global atomic revert, principal guarantee/protection, insurance, or compliance implication; open provider competition/specification/switching; no formal 6G claim.

## Mechanism state reproduced

- Route Diversity: `EXISTING / PARTIAL`, baseline only.
- Sequential Failover: `SELECT-LIMITED`; pre-execution replacement first.
- Smart-Swap Split: `EXISTING / PARTIAL`; broader extension separately measured.
- Redundant/Hedged Execution: `WATCH / DEFAULT-OFF`.

No generic `multi-path reliability`, global atomic-revert, or principal-guarantee claim exists.

## Decision ledger reproduced

| ID | Candidate state | Owner decision |
|---|---|---|
| `BM2-MP-D-0001` | Four mechanisms remain separate with independent outcomes | `false` |
| `BM2-MP-D-0002` | Sequential Failover is SELECT-LIMITED and pre-execution-first | `false` |
| `BM2-MP-D-0003` | Route/Split are existing baselines; Hedge is WATCH/default-off | `false` |

No channel-sealed, CH-00-reviewed, Owner-decided, or integrated BM2-MP decision exists.

## Owner-directed response and memory protocol

The Owner issued a process instruction, effective immediately:

1. Divide CH-04 into stable, detailed topic IDs.
2. Explain the active topic in plain language first, then in technical/hardcore depth.
3. Tag Owner questions and decision points separately from design questions, source gaps, Candidate recommendations, and hard locks.
4. Append a compact CH-04 topic tracker to every substantive response.
5. Preserve material changes in channel memory without converting discussion into completion or semantic approval.

This is `OWNER_EXPLICIT_OPERATIONAL_DIRECTION`; it is not a new `BM2-MP-D` mechanism decision.

Stable topic range: `MP-00` through `MP-23`.
Tagged question/decision range: `OQ-MP-01` through `OQ-MP-13`.
The full topic index is in `MEMORY.md`; the full tagged register is in `OPEN_QUESTIONS.md`.

## Mandatory invariants

Unique execution ID; route-plan hash; per-leg amount/exposure cap; leg states; aggregate-completion rule; last-known asset location; duplicate suppression; recovery owner/deadline; capital release; compensation reference.

## Current work and next action

1. Close `BM2-MP-01` existing/partial/new taxonomy.
2. Define `BM2-MP-02` state machine, `BM2-MP-03` idempotency, and `BM2-MP-04` recovery/location.
3. Measure `BM2-MP-05` net route value.
4. Ask for independent Go/Hold/Kill at `BM2-MP-06` only after evidence exists.

Do not begin implementation, pilot, live failover, or hedge execution. CH-00 receives only the structured handoff fields defined in `CHANNEL.md`, with a new Decision ID and exact evidence.

## Persistence status

- Candidate authoring branch only: `bm-master/ch04-topic-map-response-protocol-20260829`.
- No direct main push.
- `DECISIONS.jsonl` unchanged.
- PMO integration/persistence is required only if this operating-memory update is to become current main state.
