# Common Runtime View — Bootstrap Candidate

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
TASK_ID = COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829
STATE = VALIDATED D0 CANDIDATE / S5 PR AND READBACK
CURRENT_TASK_PERSONA_LOCK = PMO
SEMANTIC_AUTHORITY = BM_MASTER
BASE_MAIN_SHA = a3b18e231e5e3c7c053d3a838e4047ea218e4aa2
INTEGRATION_BRANCH = task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829
LANE_INTEGRATION_HEAD = f482e23980d91d04a26e83e25157dc9966f4cf7a
VALIDATION_CLAIM = PASS / EXACT D0 ONLY
OWNER_ACTION_REQUIRED = FALSE
```

## Always know

- This is an independent proposal repository, not an official Hub roadmap or
  governance decision.
- BM_MASTER owns BM semantics and Owner-facing integration; PMO owns bounded
  execution and persistence.
- BM_MASTER and PMO are the only persistent Personas. Validation is a temporary,
  task-scoped independent role after D0.
- The v1.1 proposal remains `CANDIDATE`; STEP 3–5 remains
  `OWNER-REVIEW CANDIDATE`; OR-01–OR-09 remain `UNDECIDED`.
- Four-BM order, Thin Core/Rich Edges, and every project hard lock are preserved.
- Git current state and exact evidence outrank memory, worklogs, handoffs, or
  chat. Conflict means `REVIEW_REQUIRED`.
- A local candidate, commit, merge, progress report, or bootstrap does not imply
  Owner acceptance, activation, production, implementation, or validation PASS.

## Default runtime loadout

1. Read the current Git branch/head, then repository-root `COSMOS_BM_BOOTSTRAP_CURRENT.json`.
2. Read `PROJECT_CURRENT_STATE.md` and `PROJECT_CONFIG.yaml`.
3. Load `AUTHORITY_CONTRACT.md`, this common runtime view,
   `COMMON_EXECUTION_GUARD.md`, `CHANNEL_REGISTRY.json`, and `MEMORY_INDEX.json`.
4. Resolve the current Persona only to `BM_MASTER` or `PMO`.
5. Load the selected Persona's `MEMORY.md` and `WORKLOG.md` through
   `MEMORY_INDEX.json`.
6. Load `CURRENT_TASK_BLOCKER_REGISTRY.json` and the exact task `TASK.md` and
   `PLAN.md`.
7. Load the relevant channel's current memory/decision/handoff set and only the
   exact source references required for the action.
8. State `CURRENT_PERSONA_LOCK` before material work.

A Persona lock routes the task; it does not transfer or enlarge authority.

## Narrow-first read order

```text
CURRENT POINTERS
→ EXACT TASK AND TARGET
→ EXACT SOURCE REFS
→ CHANGED PATHS / AFFECTED DIFF
→ REQUIRED DEPENDENCY NEIGHBORHOOD
→ BROADER HISTORY OR REPOSITORY SCAN ONLY WHEN A DECLARED CRITERION REQUIRES IT
```

At pre-freeze and pre-completion, perform a bounded current-state readback.
Record base/current refs, relevant pointer or task changes, semantic impact, and
the resulting action. An unrelated concurrent change is not an automatic global
rerun.

## Current task view

| Item | Current value |
|---|---|
| Task class | Full-bounded public repository/memory bootstrap |
| Authoring lanes | 4 isolated lanes, all repository-merged as Candidate inputs |
| Planned validation lanes | 1 task-scoped independent lane after D0 |
| Current planned stage | S5 / receipt persistence, PR/merge, and post-merge readback |
| Source intake | 26/26 allowlisted; 0 missing or held |
| Expected active wall | 90–180 minutes for the overall task |
| Owner check limit | 240 minutes projected active wall |
| Default correction loop | One bounded batch plus affected-diff recheck |
| Current blocker | None; D0 PASS complete, PR/merge/readback pending |
| Scope expansion | None |

PMO is the integration-branch single writer. Repository lane merge is distinct
from semantic `INTEGRATED`, Owner acceptance, validation PASS, and activation.

## Progress checkpoint format

```text
PROGRESS = [████░░░░░░] 40%
CURRENT_STAGE =
COMPLETED =
NOW =
REMAINING =
ACTIVE_WORKERS =
ACTIVE_VALIDATOR =
BASE_MAIN_SHA =
CURRENT_BRANCH_HEAD =
SOURCE_FILES_FOUND / MISSING =
STAGE_ELAPSED =
STAGE_EXPECTED =
OWNER_CHECK_LIMIT =
BLOCKER =
SCOPE_EXPANSION =
OWNER_ACTION_REQUIRED =
```

Progress comes from declared checkpoints, not elapsed time or a persuasive
estimate. If a stage or scope materially expands, report the cause and request
Owner direction where the contract reserves it.
