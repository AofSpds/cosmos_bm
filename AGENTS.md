# Repository operating contract

This repository is the Git persistence layer for the independent **COSMOS HUB
BM IMPROVEMENT** research/proposal project. It is not an official Cosmos Hub
roadmap, governance decision, product release, or production system.

## Required read order

Before substantive work, read:

1. the current Git branch and head
2. `COSMOS_BM_BOOTSTRAP_CURRENT.json`
3. `governance/v1.0/PROJECT_CURRENT_STATE.md` and `PROJECT_CONFIG.yaml`
4. `governance/v1.0/AUTHORITY_CONTRACT.md`, `COMMON_RUNTIME_VIEW.md`, and
   `COMMON_EXECUTION_GUARD.md`
5. `governance/v1.0/CHANNEL_REGISTRY.json` and `MEMORY_INDEX.json`
6. the selected `BM_MASTER` or `PMO` `MEMORY.md` and `WORKLOG.md`
7. `governance/v1.0/CURRENT_TASK_BLOCKER_REGISTRY.json` and the current task
   `TASK.md` and `PLAN.md`
8. the relevant channel `CHANNEL.md`, `MEMORY.md`, `DECISIONS.jsonl`, and
   `HANDOFF_CURRENT.md`
9. exact source files and hashes cited by the work

Git-persisted current state and exact source evidence outrank stale handoffs,
memory summaries, or chat inference. A handoff is derived context only.

## Authority and role boundary

- The Owner's latest explicit decision has highest authority.
- `BM_MASTER` is the Owner-facing semantic and BM-integration authority.
- `PMO` has bounded execution, coordination, and persistence authority only.
- The only persistent Personas are `BM_MASTER` and `PMO`.
- Validation is task-scoped and independent after a D0 freeze; do not create a
  persistent validator Persona or let PMO self-grant validation PASS.
- Never infer an Owner decision. Preserve `CANDIDATE`, `OWNER_DECIDED`, and
  `INTEGRATED` as distinct states with exact evidence for promotion.

## Current scope locks

Preserve the four BM order and every hard lock in
`governance/v1.0/PROJECT_CONFIG.yaml`. In particular, this bootstrap does not
authorize a full v1.2 rewrite, production, live routing or financial execution,
a commercial SLA or compensation promise, a native module, a fifth BM, or a
formal 6G conformity claim.

Raw source files are byte-preserved inputs. Do not rewrite them, substitute a
reconstruction for a missing original, or publish files outside the explicit
task allowlist. Derived text must be identified as non-authoritative and carry
extractor provenance.

## Memory and ledger discipline

- `MEMORY.md` is a concise current-state projection, not a transcript.
- `WORKLOG.md`, `DECISIONS.jsonl`, and the Owner decision register are
  append-only.
- `HANDOFF_CURRENT.md` is regenerated from current Git state and has no
  independent authority.
- Record exact paths, hashes, decision evidence, and Git refs when available.
- Do not relabel v1.1 or STEP 3–5 beyond their recorded candidate status.

## Task and Git discipline

Current bootstrap task:
`COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829`.

Base main SHA:
`a3b18e231e5e3c7c053d3a838e4047ea218e4aa2`.

Integration branch:
`task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829`.

Use isolated task branches/worktrees and the write surface assigned in the
task plan. Do not force-push, rewrite history, delete source files during the
bootstrap, or change another lane's paths. PMO is the single writer for final
shared-governance reconciliation on the integration branch.
