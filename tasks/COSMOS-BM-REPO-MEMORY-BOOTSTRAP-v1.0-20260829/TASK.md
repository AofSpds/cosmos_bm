# Task — Repository and Memory Bootstrap v1.0

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
TASK_ID = COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829
TASK_CLASS = FULL-BOUNDED PUBLIC REPOSITORY / MEMORY BOOTSTRAP
OWNER_DECISION = APPROVE AND EXECUTE EXACT BOUNDED TASK
TASK_STATE = IN_PROGRESS / S5 VALIDATED D0 / PR PENDING
CURRENT_PERSONA_LOCK = PMO
SEMANTIC_AUTHORITY = BM_MASTER
BASE_MAIN_SHA = a3b18e231e5e3c7c053d3a838e4047ea218e4aa2
INTEGRATION_BRANCH = task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829
VALIDATION_CLAIM = PASS / EXACT D0 ONLY
OWNER_ACTION_REQUIRED = FALSE
```

## Mission

Initialize `AofSpds/cosmos_bm` as the Git persistence layer for project
governance and pointers, BM_MASTER/PMO memory, eight specialist-channel current
sets, exact allowlisted sources, the STEP 3–5 Owner-review candidate package,
channel policy packets, and future Git-backed succession.

This is repository and memory-governance bootstrap work. It is not proposal
revision, new research, product implementation, production deployment, live
routing, or an official Cosmos Hub decision.

## Exact authorization

The Owner authorizes:

- this bounded bootstrap task;
- publication of only the packet's exact source allowlist after integrity and
  publication prechecks;
- four isolated authoring lanes and PMO single-writer integration;
- one task-scoped independent validating lane after D0;
- one bounded correction batch and affected-diff recheck by default.

The authorization preserves the four-BM order and every common hard lock. It
does not approve OR-01–OR-09, the candidate concept portfolio, a full v1.2
rewrite, production, live routing/financial execution, commercial SLA or
compensation, native module, fifth BM, formal 6G conformity, additional
persistent Personas, or a repository license.

## Fixed Git topology

| Purpose | Exact branch/ref |
|---|---|
| Base main | `a3b18e231e5e3c7c053d3a838e4047ea218e4aa2` |
| Integration | `task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829` |
| Lane A — governance | `task/bootstrap/governance-core-20260829` |
| Lane B — sources | `task/bootstrap/source-ingest-20260829` |
| Lane C — channels 00–03 | `task/bootstrap/channels-00-03-20260829` |
| Lane D — channels 04–07 | `task/bootstrap/channels-04-07-20260829` |

All lane branches start at the exact base. Each uses an isolated worktree and
write surface. No force push, history rewrite, shared-path race, or direct
post-genesis main write is authorized.

## Authoring lanes

Wave 1 authoring is complete. The lane scope descriptions below are retained as
historical write-boundary evidence.

### Lane A — Governance core

May write only:

- `AGENTS.md`
- candidate `COSMOS_BM_BOOTSTRAP_CURRENT.json`
- `governance/v1.0/**`, containing exactly the structure specified by the task
  packet and only the persistent Persona directories `BM_MASTER` and `PMO`
- this task's `TASK.md` and `PLAN.md`

It must not write sources, channels, README, `.gitignore`, `.gitattributes`, a
lane report, validation receipt, outputs, completion file, or other lane paths.

### Lane B — Source ingest

Owns `sources/**` and `lane-reports/SOURCE_INGEST.md`; performs exact allowlist,
hash/byte, archive, credential/PII/metadata, openability, and publication checks.

### Lane C — Channels 00–03

Owns the channel directories for integration-owner,
distribution-market-revenue, observability-slo-sla, and
ai-assisted-skip-go-routing plus its lane report.

### Lane D — Channels 04–07

Owns the channel directories for failover-recovery-design,
enterprise-gateway-structured-intent, asset-service-registry, and
legal-governance-economics plus its lane report.

PMO alone reconciles final shared governance indexes on the integration branch.

## Required state semantics

- v1.1 remains `CANDIDATE / independent proposal / not official Hub policy`.
- STEP 3–5 remains `OWNER-REVIEW CANDIDATE`.
- Overall classification remains `B. SELECTIVE FIT — CANDIDATE`.
- OR-01–OR-09 remain `UNDECIDED / DO NOT AUTO-INFER`.
- MEMORY is compressed current state; WORKLOG and decisions are append-only;
  HANDOFF_CURRENT is derived succession context with no independent authority.
- Only BM_MASTER and PMO are persistent Personas. Validation is task-scoped and
  independent.

## Structural checks

1. S01 — Parse every JSON file.
2. S02 — Parse every YAML file.
3. S03 — Resolve all bootstrap pointers.
4. S04 — Confirm exactly eight unique channel IDs.
5. S05 — Confirm unique slugs and decision prefixes.
6. S06 — Confirm exactly two persistent Personas: BM_MASTER and PMO.
7. S07 — Confirm seven required core files in every channel.
8. S08 — Match every raw import to recorded SHA-256 and byte count.
9. S09 — Match ZIP members to expected package contents.
10. S10 — Confirm no non-allowlisted source is committed.
11. S11 — Confirm no unresolved secret/credential finding.
12. S12 — Confirm no raw PII/KYC or unrelated Library content.
13. S13 — Confirm no unsupported `OWNER_DECIDED`/`INTEGRATED` state.
14. S14 — Confirm no unauthorized production/rewrite/live/native claim.
15. S15 — Confirm no broken exact source or Git refs in current-state files.
16. S16 — Confirm HANDOFF_CURRENT reproduces memory/decision state.
17. S17 — Confirm README candidate/non-official status and read order.
18. S18 — Confirm no license selected without an Owner decision.

Lane checks are scoped; PMO runs the complete S01–S18 set after all merges and
before D0.

## Acceptance criteria

| ID | Criterion |
|---|---|
| AC-00 | Exact Git baseline, branch map, and repository state recorded |
| AC-01 | Available allowlisted sources imported byte-identically, hashed, manifested; missing desired sources recorded |
| AC-02 | No secret, unrelated export, token, KYC/PII, or non-allowlisted publication |
| AC-03 | Root/config/authority/runtime/state/task/decision-register artifacts exist and parse |
| AC-04 | Only BM_MASTER and PMO persist; PMO has execution, not semantic/validation authority |
| AC-05 | Eight stable channels with seven required files each |
| AC-06 | Candidate and undecided states preserved; no unauthorized implementation/production claim |
| AC-07 | MEMORY, append-only logs/decisions, and derived handoffs obey their distinct semantics |
| AC-08 | Raw sources preserved; derived text is non-authoritative with provenance |
| AC-09 | Isolated branches/worktrees and write surfaces avoid races/lost updates |
| AC-10 | Independent validation receipt bound to exact D0/D1; PMO does not self-validate |
| AC-11 | PR/merge or HOLD, exact refs, readback, task completion, and handoffs recorded |
| AC-12 | No new research, rewrite, implementation, or Persona system silently added |

## Validation and completion boundary

Only after PMO integrates all four lanes, reconciles shared paths, and passes
the structural checks may it freeze D0 and dispatch the single independent
task-scoped validator. The validator cannot edit or merge. Findings freeze as
blocking, advisory, or new-scope. One correction batch and affected recheck is
the default.

Keep `AUTHORING_COMPLETE`, `STRUCTURAL_CHECK_COMPLETE`,
`VALIDATION_COMPLETE`, `COMMITTED`, `MERGED`, `PERSISTENCE_COMPLETE`,
`OWNER_ACCEPTED`, and `ACTIVATED` separate. Exact-D0 validation PASS exists;
main merge, persistence completion, Owner acceptance, and activation remain
absent.

## Current exact checkpoint

- `AUTHORING_COMPLETE = TRUE` — exact lane commits are recorded in
  `governance/v1.0/INTEGRATION_STATUS.md`.
- `STRUCTURAL_CHECK_COMPLETE = TRUE` — final pre-freeze S01–S18 passed 18/18.
- `VALIDATION_COMPLETE = TRUE` for exact D0
  `7de27f727582c4626c76728fbdf4196b40007591`; no findings required correction,
  so `D1 = NOT REQUIRED`.
- `COMMITTED = TRUE` for exact D0 and validation-receipt persistence is the
  current administrative step.
- `MERGED = FALSE` for main; repository lane merge is only integration-branch
  lineage.
- `PERSISTENCE_COMPLETE = FALSE`, `OWNER_ACCEPTED = FALSE`, and
  `ACTIVATED = FALSE`.
- Source intake is 26/26 allowlisted files with 0 missing or held.
