# Integration Status — Lane A Candidate

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
TASK_ID = COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829
BASE_MAIN_SHA = a3b18e231e5e3c7c053d3a838e4047ea218e4aa2
INTEGRATION_BRANCH = task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829
LANE_A_BRANCH = task/bootstrap/governance-core-20260829
CURRENT_PLANNED_STAGE = S2 / WAVE 1 / PARALLEL AUTHORING
LANE_A_STATE = CANDIDATE / NOT YET MERGED
D0 = NOT CREATED
D1 = NOT CREATED
VALIDATION = NOT STARTED
OWNER_ACCEPTED = FALSE
ACTIVATED = FALSE
```

## Lane view

| Lane | Expected surface | Status visible to Lane A |
|---|---|---|
| A — governance core | Root agent/pointer, `governance/v1.0/**`, task `TASK.md` and `PLAN.md` | Authoring candidate on isolated branch |
| B — source ingest | `sources/**`, source-ingest lane report | Not assessed from this lane |
| C — channels 00–03 | Four channel directories and lane report | Not assessed from this lane |
| D — channels 04–07 | Four channel directories and lane report | Not assessed from this lane |

Lane A does not infer the completion, source availability, publication safety,
or commit state of another lane. PMO must read exact lane commits before
changing these statuses.

## Candidate governance outcome

Lane A prepares:

- the narrow repository operating contract and candidate current pointer;
- project config, current state, authority contract, runtime view, and execution
  guard;
- candidate channel registry and memory index;
- current task/blocker and sole Owner authorization registers;
- exactly two persistent Persona memory/worklog directories;
- task definition and execution plan.

The channel paths in the candidate indexes remain explicitly pending until the
corresponding channel lanes are merged and PMO verifies every pointer.

## PMO integration order

1. Merge Lane A governance-core candidate.
2. Merge Lane B source-ingest candidate.
3. Merge Lane C channels 00–03 candidate.
4. Merge Lane D channels 04–07 candidate.
5. Reconcile all shared paths, hashes, source availability, registry resolution
   states, current task status, and exact Git refs as a single writer.
6. Run structural checks S01–S18 and record exact output.
7. Freeze D0; only then dispatch the independent task-scoped validator.
8. Classify frozen findings and, if needed, apply one bounded correction batch,
   freeze D1, and request affected-diff recheck.
9. Continue to PR/merge/readback only after the applicable gates pass.

## Current next action

Lane A runs format, content, path-scope, and Git-diff checks, creates one local
candidate commit, and returns its exact SHA and changed-file list to PMO. A
local Lane A commit does not constitute D0, integration, validation,
persistence completion, Owner acceptance, or activation.
