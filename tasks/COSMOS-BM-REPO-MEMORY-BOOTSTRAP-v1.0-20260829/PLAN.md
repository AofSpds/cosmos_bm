# Plan — Repository and Memory Bootstrap v1.0

```text
TASK_ID = COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829
BASE_MAIN_SHA = a3b18e231e5e3c7c053d3a838e4047ea218e4aa2
INTEGRATION_BRANCH = task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829
CURRENT_PLANNED_STAGE = S2 / WAVE 1 / PARALLEL AUTHORING
PLANNED_AUTHORING_WORKERS = 4
PLANNED_VALIDATING_WORKERS = 1 TASK-SCOPED AFTER D0
EXPECTED_ACTIVE_WALL = 90–180 MINUTES
OWNER_CHECK_LIMIT = 240 MINUTES PROJECTED ACTIVE WALL
DEFAULT_CORRECTION_LOOP = ONE BOUNDED BATCH + AFFECTED-DIFF RECHECK
VALIDATION_CLAIM = NONE
```

## Stage plan

| Stage | Weight | Expected range | Current disposition |
|---|---:|---:|---|
| S0 — admission, Git/source readback | 10% | 10–20 min | Base and packet read back for Lane A; overall source result belongs to PMO/Lane B |
| S1 — genesis, branches, worktrees | 10% | 10–20 min | Genesis base and Lane A branch/worktree verified; PMO owns overall branch map |
| S2 — parallel Wave 1 authoring | 40% | 30–60 min | **Current planned stage** |
| S3 — PMO integration and structural checks | 20% | 20–40 min | Pending all lane commits |
| S4 — independent task-scoped validation | 10% | 15–30 min | Pending exact D0 freeze |
| S5 — correction/recheck/PR/merge/readback | 10% | 15–30 min | Pending validation disposition |

Ranges are anomaly detectors, not deadlines. Heartbeat every 10–15 minutes.
After about 20 minutes without material progress, diagnose once and retry once;
if still stalled, checkpoint and stop the affected lane. Report a freeze or
readback unexpectedly over about 30 minutes rather than spin silently.

## Wave 1 authoring map

| Lane | Branch | Isolated write surface |
|---|---|---|
| A — governance core | `task/bootstrap/governance-core-20260829` | `AGENTS.md`, candidate root pointer, `governance/v1.0/**`, task `TASK.md`/`PLAN.md` |
| B — source ingest | `task/bootstrap/source-ingest-20260829` | `sources/**`, source lane report |
| C — channels 00–03 | `task/bootstrap/channels-00-03-20260829` | Four assigned channel directories, lane report |
| D — channels 04–07 | `task/bootstrap/channels-04-07-20260829` | Four assigned channel directories, lane report |

No lane writes another lane's path. PMO is the only integration-branch writer
for final shared indexes and exact current pointers.

## Lane A work plan

1. Read the complete sole execution packet and verify exact base, branch,
   worktree, and clean status.
2. If locally available, consult only Byul's concise pointer, narrow-read,
   current MEMORY, append-only WORKLOG, progress, and freeze/recheck conventions;
   do not import its Persona or validator organization.
3. Author only the assigned 18 files:
   - root `AGENTS.md` and candidate current pointer;
   - the exact 14-file governance v1.0 structure specified by the packet;
   - task `TASK.md` and `PLAN.md`.
4. Seed only the explicit bounded-bootstrap Owner authorization.
5. Preserve the four BMs, all hard locks, v1.1 and STEP 3–5 candidate states,
   OR-01–OR-09 undecided status, and all negative authorization boundaries.
6. Run Lane A scoped parse, uniqueness, Persona-count, pointer, forbidden-claim,
   write-surface, and whitespace checks.
7. Review the exact diff, create one local candidate commit, and return the SHA,
   changed files, checks, and any advisory/blocker to PMO.

## Lane A scoped checks

- Parse every authored `.json` and every nonblank JSONL line.
- Parse `PROJECT_CONFIG.yaml`.
- Confirm channel ID count 8 and uniqueness of IDs, slugs, and decision prefixes.
- Confirm only `governance/v1.0/personas/BM_MASTER` and
  `governance/v1.0/personas/PMO` exist.
- Confirm all candidate root/governance/task pointers owned by Lane A resolve;
  channel-memory pointers must remain explicitly `PENDING_CHANNEL_LANE_MERGE`.
- Confirm `OWNER_DECISION_REGISTER.jsonl` has exactly one seed entry and
  OR-01–OR-09 remain undecided.
- Search for unauthorized state promotion, activation, production, live routing,
  commercial SLA, native-module, fifth-BM, and formal-6G claims.
- Confirm changed paths stay inside Lane A's allowlist.
- Run `git diff --check` and inspect the final staged diff.

Passing Lane A checks produces only a local authoring candidate. Full S01–S18,
publication safety, channel completeness, D0/D1 validation, and persistence
remain PMO/integration responsibilities.

## Wave 2 — PMO integration

Merge lanes A, B, C, then D. Reconcile exact source hashes/statuses, channel and
memory paths, blocker/task state, Owner register, project state, Persona
memories/worklogs, and generated handoffs. Run S01–S18. Perform a bounded
current-state readback and freeze an exact D0 only when the candidate is stable.

## Wave 3 — independent validation

Dispatch one temporary independent validating worker under Appendix A of the
sole packet. Provide D0, base, branch, changed list, allowlist/manifests/checks,
governance artifacts, channel current sets, and AC-00–AC-12. The validator must
not edit, merge, create decisions, or redesign scope.

## Waves 4–5 — correction and persistence

Freeze findings as blocking/advisory/new-scope. PMO applies one bounded
correction batch by default, freezes D1, and requests only affected-diff/
affected-criterion recheck unless material-global impact is proven. Then open
the integration PR, merge only after gates pass, perform post-merge exact
readback, update completion/handoffs, and report final refs. Otherwise record an
explicit HOLD.

## Current progress snapshot

```text
PROGRESS = [██░░░░░░░░] 20% OVERALL CHECKPOINT FLOOR AT S2 ENTRY
CURRENT_STAGE = S2 / WAVE 1 / PARALLEL AUTHORING
COMPLETED = S0/S1 BASE AND LANE A WORKTREE READBACK
NOW = LANE A GOVERNANCE-CORE AUTHORING AND SCOPED CHECKS
REMAINING = LANE COMMITS / PMO INTEGRATION / S01-S18 / D0 / VALIDATION / CORRECTION IF ANY / PERSISTENCE
ACTIVE_WORKERS = 4 PLANNED AUTHORING LANES; ACTUAL OVERALL COUNT RECONCILED BY PMO
ACTIVE_VALIDATOR = NONE; ONE PLANNED ONLY AFTER D0
BASE_MAIN_SHA = a3b18e231e5e3c7c053d3a838e4047ea218e4aa2
CURRENT_BRANCH_HEAD = LANE COMMIT NOT YET RECORDED IN THIS CANDIDATE PLAN
SOURCE_FILES_FOUND / MISSING = OWNED BY SOURCE-INGEST LANE / NOT INFERRED HERE
BLOCKER = NONE RECORDED FOR LANE A
SCOPE_EXPANSION = NONE
OWNER_ACTION_REQUIRED = FALSE
NEXT_EXACT_ACTION = COMPLETE LANE A CHECKS AND LOCAL COMMIT; RETURN EXACT SHA TO PMO
```

This snapshot must be reconciled by PMO from exact current Git and lane results;
it does not claim overall task completion.
