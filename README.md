# Cosmos Hub BM Improvement

> INDEPENDENT RESEARCH / CANDIDATE / NO PRODUCT AUTHORITY

This repository is the Git persistence layer for an independent Cosmos Hub
business-model research and proposal project. It is not an official Cosmos Hub
roadmap, governance decision, product commitment, or production system.

## Current baseline

| Surface | Current state |
|---|---|
| Proposal | **v1.1 Candidate** |
| Roadmap package | **STEP 3–5 Owner-review Candidate** |
| Overall classification | **B. Selective Fit — Candidate** |
| Owner queue `OR-01`–`OR-09` | **Undecided; do not infer** |

No production deployment, live routing or financial execution, commercial
SLA, compensation, insurance, principal guarantee, native module, full v1.2
rewrite, fifth BM, or formal 6G conformity is authorized by this repository.

## Bootstrap read order

1. Read the current Git branch/head; current Git state outranks stale memory or
   handoff text.
2. Read `COSMOS_BM_BOOTSTRAP_CURRENT.json`.
3. Read `governance/v1.0/PROJECT_CURRENT_STATE.md`,
   `PROJECT_CONFIG.yaml`, `AUTHORITY_CONTRACT.md`, `COMMON_RUNTIME_VIEW.md`,
   `COMMON_EXECUTION_GUARD.md`, `CHANNEL_REGISTRY.json`, and
   `MEMORY_INDEX.json`.
4. Resolve only `BM_MASTER` or `PMO`, then read that Persona's current
   `MEMORY.md` and append-only `WORKLOG.md`.
5. Read the current task, blocker registry, and exact Git/source references.
6. Read only the relevant channel's seven-file current set, with
   `HANDOFF_CURRENT.md` treated as derived succession context.
7. Verify claims against exact files in `sources/raw/` or `sources/packages/`.

## Channels

| Stable ID | Display name | Git path |
|---|---|---|
| `CH-00` | INTEGRATION · OWNER | `channels/integration-owner/` |
| `CH-01` | DISTRIBUTION · REVENUE | `channels/distribution-market-revenue/` |
| `CH-02` | OBSERVABILITY · SLA | `channels/observability-slo-sla/` |
| `CH-03` | AI ROUTING · SKIP GO | `channels/ai-assisted-skip-go-routing/` |
| `CH-04` | FAILOVER · RECOVERY | `channels/failover-recovery-design/` |
| `CH-05` | GATEWAY · INTENT | `channels/enterprise-gateway-structured-intent/` |
| `CH-06` | REGISTRY · PROVIDERS | `channels/asset-service-registry/` |
| `CH-07` | LEGAL · GOV · ECON · CLAIMS | `channels/legal-governance-economics/` |

Stable channel IDs and slugs in
`governance/v1.0/CHANNEL_REGISTRY.json` are canonical; display labels are
convenience labels only.

## Source authority

Files under `sources/raw/` and `sources/packages/` are byte-preserved,
allowlisted inputs recorded in `sources/SOURCE_MANIFEST.yaml` and
`sources/SHA256SUMS.txt`. Any future extraction belongs under
`sources/derived/`, must identify its source hash and extractor version, and is
non-authoritative. Derived text never substitutes for a missing original.

## License

No repository license has been selected. A license requires a separate, exact
Owner decision.
