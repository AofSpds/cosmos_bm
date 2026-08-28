# CH-06 Current Handoff

`ARTIFACT_CLASS = DERIVED CONTEXT ONLY / NO INDEPENDENT AUTHORITY`

Regenerate from current Git, memory, decisions, and open questions after material change. Higher-authority Owner, CH-00, and charter records prevail.

GENERATION_STAGE = `PRE_D0_INTEGRATION_RECONCILIATION`
TASK_ID = `COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829`
INTEGRATION_BRANCH = `task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829`
DERIVED_INPUTS = `MEMORY.md + DECISIONS.jsonl + OPEN_QUESTIONS.md`

FROM_CHANNEL = `CH-06 — ASSET & SERVICE REGISTRY`
DECISION_ID = `BM4-REG-D-0001`
STATUS = `CANDIDATE / NOT CHANNEL-SEALED / NO OWNER DECISION`
QUESTION = How can a factual asset/provider registry support discovery without implying approval, safety, ranking authority, or compliance?
RECOMMENDED_DECISION = Separate declarations, verification evidence, factual capability records, deterministic eligibility, and model ranking while preserving freshness and revocation.
ALTERNATIVES_CONSIDERED = Approval badges, eligibility/ranking conflation, closed entry, raw public KYC/PII, and a mandatory operator/router; excluded by hard locks.
EVIDENCE = Exact CH-06 packet SHA-256 `17cb30af452ec3eb38b878d20503fccc01766b5bed189730f41e317600a7c437`; current source hashes in `SOURCES.md`.
RATIONALE = Registry facts require source, time, freshness, confidence, missingness, incident, and revocation provenance and cannot create a guarantee.
IMPACTED_CHANNELS = CH-01 attribution, CH-02 evidence, CH-03 provider health, CH-04 route/failover, CH-05 service mapping, CH-07 competition/data/claims, CH-00 promotion
IMPACTED_BM = BM4 directly; factual provider interfaces for BM1–BM3
IMPACTED_TRACK = Pre-PoC asset/provider schema, freshness/revocation, eligibility/ranking, and open-entry evidence
HARD_LOCK_CHECK = Preserved; factual registry only, no safety/compliance guarantee, raw public PII, closed market, or mandatory router
DEPENDENCIES = Issuer/provider schema; signature and verification provenance; incident/revocation semantics; deterministic eligibility; public arbitration
LEGAL_SAFETY_ECONOMIC_EFFECT = None authorized; listing, verification, liability, discrimination, concentration, and fee questions remain unresolved
CLAIM_CEILING = `C2 — pre-PoC maximum`
OWNER_ACTION_REQUIRED = `FALSE` now; `TRUE` only when a bounded registry, eligibility, or pilot choice is ready
PROPOSED_INTEGRATION = None until `BM4-REG-01`–`06` close and a channel-sealed handoff is submitted
SUPERSEDES = None

## Identity and read order

- Channel: `CH-06 ASSET & SERVICE REGISTRY`
- Slug / prefix: `asset-service-registry` / `BM4-REG-D`
- Charter: `sources/raw/channel-policy-packets/v1.0/06_CH06_BM4_REGISTRY_PROVIDER_MARKET_PACKET.md`
- SHA-256: `17cb30af452ec3eb38b878d20503fccc01766b5bed189730f41e317600a7c437`
- Read: current Git/governance → `CHANNEL.md` → `MEMORY.md` → `DECISIONS.jsonl` → `OPEN_QUESTIONS.md` → `SOURCES.md` → `WORKLOG.md` → this handoff.

## Current state reproduced

- v1.1 Candidate, independent, not official Hub policy; STEP 3–5 Owner-review Candidate.
- `B. SELECTIVE FIT` and portfolio dispositions remain Candidate; OR-01–OR-09 are UNDECIDED.
- C2 is the current pre-PoC ceiling.
- Production, full rewrite, fifth BM, native module, live routing/financial execution, commercial SLA/compensation, and formal 6G conformity are not authorized.

Locked BM order: Distribution Market → Assured Delivery SLA → Enterprise Gateway → Asset & Service Registry.

Hard locks: Thin Core/Rich Edges; open base IBC/no forced Hub toll; no Hub principal custody/mandatory ATOM; no Hub DEX/bridge/lending/perp/stablecoin/market making/proprietary mandatory router; no public raw KYC/PII/sensitive policy; contract/data and small audited CosmWasm first; no AI keys/authorization/hard-policy mutation/unilateral compensation; no global atomic revert/principal guarantee/insurance/compliance implication; open competition/public specification/switching; no formal 6G claim.

## Channel state reproduced

- Registry is factual evidence, not approval/safety/guarantee/compliance.
- Separate issuer declaration/verification, provider self-report/independent evidence, capability/score, and deterministic eligibility/model ranking.
- Show signature, source, time, freshness, version, confidence, missingness, incident scope/resolution, and revocation.
- Keep sensitive details off-chain and preserve open entry, switching, newcomer evaluation, concentration controls, public arbitration, and no mandatory operator/router.

## Decision ledger reproduced

| ID | Candidate state | Owner decision |
|---|---|---|
| `BM4-REG-D-0001` | Registry is factual only; approval/safety/compliance labels prohibited | `false` |
| `BM4-REG-D-0002` | Eligibility is deterministic and separate from ranking; arbitration is public/deterministic | `false` |
| `BM4-REG-D-0003` | Open competition/switching and off-chain sensitive-data boundary apply | `false` |

No channel-sealed, CH-00-reviewed, Owner-decided, or integrated BM4-REG decision exists.

## Current work and next action

1. Close BM4-REG-01 Asset/issuer schema.
2. Close BM4-REG-02 Provider/capability schema.
3. Close BM4-REG-03 freshness/incident/revocation model.
4. Only then address eligibility/ranking, open-entry/concentration, and conflict arbitration.

Do not issue a badge, select a provider, publish sensitive data, or start a Registry implementation. Send CH-00 only the structured handoff defined in `CHANNEL.md`, with a new Decision ID and exact evidence.
