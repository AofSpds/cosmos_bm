# Common Execution Guard — v1.0 Bootstrap Candidate

```text
ARTIFACT_ID = COSMOS-BM-COMMON-EXECUTION-GUARD-v1.0
PROJECT = COSMOS HUB BM IMPROVEMENT
TASK_ID = COSMOS-BM-REPO-MEMORY-BOOTSTRAP-v1.0-20260829
STATE = CANDIDATE / PENDING PMO INTEGRATION
SCOPE = BM_MASTER AND PMO
VALIDATION_CLAIM = NONE
AUTHORITY_CHANGE = NONE
```

This guard governs task opening, narrow Git reads, isolated authoring,
progress, D0/D1 freezes, independent validation, correction, and persistence.
It does not create semantic authority, an Owner decision, a validation PASS, or
production authority.

## 1. Core operating rule

Quality and correctness remain required. Silent scope expansion, unexplained
long work, shared-path races, repeated whole-target reads, and unbounded
revalidation are not allowed. Estimates are anomaly detectors rather than
forced deadlines.

## 2. Task opening

Before substantive work, establish:

- task class, exact authorization, and acceptance criteria;
- base SHA, branch/worktree, current pointer, and assigned write surface;
- stage budgets, progress weights, Owner check limit, workers, and validator;
- exact read scope and correction-loop expectation;
- blockers, scope expansion, and Owner action required.

Read current pointers and exact targets before broad repository exploration.
State the current Persona lock. If Git current state conflicts materially with
memory, handoff, or chat, declare `REVIEW_REQUIRED` rather than guessing.

## 3. Narrow-first and bounded readback

Read in this order: current pointers, exact task/target, exact source refs,
affected diff, required dependency neighborhood, then wider history only when a
declared acceptance criterion requires it. A wider or repeated scan must name
the criterion, scope, and extra work.

For a frozen candidate or persistence result, do bounded readbacks immediately
before freeze and completion. Record base and current refs, relevant changes,
semantic impact, and action. Synchronize only the affected area unless a
material-global finding proves a wider recheck is necessary.

## 4. Lane and Git isolation

- All four authoring lanes begin at
  `a3b18e231e5e3c7c053d3a838e4047ea218e4aa2`.
- Each lane uses its assigned isolated branch/worktree and writes only its
  declared surface.
- PMO is the single writer for final shared governance reconciliation on
  `task/governance/cosmos-bm-memory-bootstrap-v1.0-20260829`.
- No force push, history rewrite, direct post-genesis main write, shared-path
  race, or bootstrap source deletion is allowed.
- Local lane commits are candidates, not activation or validation events.

Lane A may write only `AGENTS.md`, the candidate root bootstrap pointer,
`governance/v1.0/**`, and the current task's `TASK.md` and `PLAN.md`. It must not
write sources, channels, README, lane reports, validation receipts, outputs, or
completion artifacts.

## 5. Semantic, status, and Persona firewall

- BM_MASTER retains semantic authority; PMO retains execution/persistence
  authority only.
- The only persistent Personas are BM_MASTER and PMO.
- Never infer Owner decisions or promote candidate state without exact evidence.
- Keep v1.1 and STEP 3–5 at their recorded candidate classifications.
- Keep OR-01–OR-09 undecided.
- Preserve the four-BM order and every hard lock in `PROJECT_CONFIG.yaml`.
- Do not expand into a full v1.2 rewrite, new research, product implementation,
  production, live routing, commercial SLA, native module, fifth BM, or formal
  6G conformity claim.

## 6. Source and publication boundary

Source intake is exact-allowlist-only, byte-preserving, hashed, and
publication-guarded. Every raw import requires title/allowlist match, SHA-256,
byte count, type, secrets/PII/metadata review, openability, and duplicate check.
Archives require member inventory. Hold only the affected file for ambiguity,
hash mismatch, corruption, or sensitive content; do not reconstruct a missing
original under the same identity.

Raw inputs are authoritative bytes. Derived text is non-authoritative and must
record source hash, extractor, and version. Lane A does not ingest sources.

## 7. Memory and ledger discipline

- MEMORY is concise current state, never a transcript or decision source.
- WORKLOG and decision ledgers are append-only.
- HANDOFF_CURRENT is regenerated derived context with no independent authority.
- Parallel workers do not race on shared memory/worklog files.
- PMO reconciles shared indexes once on the integration branch.

## 8. Progress and stall watchdog

Overall task stage weights are S0 10%, S1 10%, S2 40%, S3 20%, S4 10%, and
S5 10%. Report checkpoints every 10–15 minutes during substantive execution.
After roughly 20 minutes without material progress, perform one diagnosis and
one bounded retry. If still stalled, persist the checkpoint, report the exact
gap, and stop the affected lane. A candidate freeze/readback unexpectedly over
roughly 30 minutes is reported rather than hidden behind a spinner.

The overall expected active wall is 90–180 minutes; the projected Owner check
limit is 240 minutes. New full scans, validators, research/design, high-impact
scope, extra correction loops, or materially larger remaining work require an
explicit anomaly report and, where reserved, Owner confirmation.

## 9. Candidate freeze and independent validation

```text
AUTHORING
→ PMO INTEGRATION AND STRUCTURAL CHECKS
→ D0 EXACT CANDIDATE FREEZE
→ ONE TASK-SCOPED INDEPENDENT VALIDATING WORKER
→ FINDING FREEZE AND CLASSIFICATION
→ ONE PMO CORRECTION BATCH BY DEFAULT
→ D1 FREEZE
→ AFFECTED-DIFF / AFFECTED-CRITERIA RECHECK
```

The validator receives the frozen SHA, exact allowlist/source refs, changed
files, structural output, authority/config/index files, eight channel current
sets, and AC-00–AC-12. It may not edit, merge, create Owner decisions, redesign
the project, or turn advisory/new-scope suggestions into gates. PMO may not
self-certify independent PASS.

Classify findings as `BLOCKING`, `ADVISORY`, or `NEW-SCOPE`. A new SHA changes
byte identity but does not itself require global revalidation. Broaden only for
a demonstrated material-global impact.

## 10. Completion and persistence

Keep these states distinct:

```text
AUTHORING_COMPLETE
STRUCTURAL_CHECK_COMPLETE
VALIDATION_COMPLETE
COMMITTED
MERGED
PERSISTENCE_COMPLETE
OWNER_ACCEPTED
ACTIVATED
```

Before persistence closure, require the exact final branch head, validation
receipt bound to the reviewed SHA, PR/merge or explicit HOLD, post-merge
readback, current task/worklog update, resolved current pointers, and exact next
action. A progress bar or local commit cannot imply a later state.

## 11. Stop and escalation conditions

Hold the task for insufficient repository permission, an unsafe base, a
material Owner-decision conflict, a required non-allowlisted publication,
failure to isolate independent validation, or an unresolved blocking
authority/structure defect after the authorized correction batch. Request Owner
confirmation for every boundary reserved in `AUTHORITY_CONTRACT.md`.
