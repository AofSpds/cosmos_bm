# CH-03 Sources

Exact canonical repository paths are used for imported project sources so the
source-ingest lane can preserve bytes independently. Live official web documents
are separately marked as non-imported snapshots. Raw/imported sources and exact
primary documents outrank this derived channel source register.

## A. Imported project and policy sources

| ID | Canonical repository path | SHA-256 | Status / authority | Use and caution |
|---|---|---|---|---|
| C04 | `sources/raw/channel-policy-packets/v1.0/03_CH03_BM2_AI_SKIP_GO_ROUTING_PACKET.md` | `8b38aa15d914f0ca95e83a337da027139d000795372f7f5cdcba6ccd25ceb7ef` | Exact standalone channel policy packet | Controlling charter input; corrected standalone hash, not an older archive copy |
| A01 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.docx` | `19f948efcc43987213bb5f71157dd17ac98fb1a88e5acc2b474bd1cc1a966610` | Candidate; independent proposal; not official Hub policy | Proposal baseline; no production/governance authority |
| A02 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.pdf` | `d71c4dea192db1facde65fce5dbc164d8586bc386438253b0b4126a13a99622b` | Rendered Candidate companion | Presentation copy; source status remains Candidate |
| A03 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.txt` | `b298db88356148798f57be5f8ea4335959c3e79d499860bd2fd81dc3f8545105` | Candidate text companion | Searchable baseline; not official policy |
| B01 | `sources/raw/v1.2-step3-5/00_OWNER_REVIEW_INDEX.md` | `c70dfbc6a4686be23fdf1b56ce32f57c3fdf538dde147e704044894d1b5a5bd1` | Owner-review Candidate | Decision summary only; no Owner approval |
| B02 | `sources/raw/v1.2-step3-5/V1.2_6G_PRIOR_ART_EVIDENCE_LEDGER.md` | `1e4397684d8c8fabc139b9a47843066a2c142ec0da277c6d7199c3f0a656f75a` | Owner-review Candidate | Prior-art/evidence context; no 6G conformity claim |
| B03 | `sources/raw/v1.2-step3-5/V1.2_6G_CONCEPT_SELECTION_MATRIX.md` | `b4c0829a71726cea5997ebd7927863979f1c34178cab51acae9e807155565dfc` | Owner-review Candidate | Bounded AI is Select-Limited Candidate; route diversity/split are existing/assess |
| B04 | `sources/raw/v1.2-step3-5/V1.2_PARALLEL_TRACK_ROADMAP_CANDIDATE.md` | `e7455c86a0382b846a8cd5034ea2215068217231beebb0eded7b63ff3e9026bc` | Owner-review Candidate | M2 Shadow and T2 work only; no live or production authority |

## B. Live official Skip Go sources for T02

Snapshot date: `2026-08-30`. These pages were reviewed as official current
product documentation. They are not yet byte-imported or hash-frozen in the
repository, so later changes require affected-claim refresh rather than silent
inheritance.

| ID | Official URL | Use | Current caution |
|---|---|---|---|
| SG-01 | `https://docs.skip.build/go/general/getting-started` | platform scope, supported integration forms and high-level capabilities | product overview; not a complete route-engine specification |
| SG-02 | `https://docs.skip.build/go/general/overview-and-typical-usage` | canonical route → msgs → submit/track → status usage flow | API behavior can change; exact request/response must be captured |
| SG-03 | `https://docs.skip.build/go/api-reference/prod/fungible/post-v2fungibleroute` | route request controls, bridge enums and response schema | server-side defaults and scoring internals are not fully versioned in the page |
| SG-04 | `https://docs.skip.build/go/api-reference/prod/fungible/post-v2fungiblemsgs_direct` | message/transaction output, minimum output and route echo | message construction is not user authorization |
| SG-05 | `https://docs.skip.build/go/advanced-transfer/ibc-routing-algorithm` | origin unwind, manual override, direct-path/liquidity and client/channel conditions | IBC denom/path algorithm is a subcomponent, not the full universal route engine |
| SG-06 | `https://docs.skip.build/go/advanced-swapping/smart-swap-options` | external routers, route splitting and EVM swaps | existing/partial capability; not generalized redundant execution |
| SG-07 | `https://docs.skip.build/go/client/executing-a-route` | user-signer integration, simulation, ordered execution and callbacks | the client uses user/integrator signer functions; no Skip key custody inferred |
| SG-08 | `https://docs.skip.build/go/advanced-transfer/interpreting-transaction-status` | overall state, transfer sequence, blocking leg and asset-release interpretation | provider API status is not automatically independent commercial adjudication |
| SG-09 | `https://docs.skip.build/go/advanced-transfer/handling-cross-chain-failure-cases` | IBC/Axelar/CCTP/Hyperlane/Go Fast failure and asset-location behavior | failure outcome is protocol-, leg- and multi-tx-specific |
| SG-10 | `https://docs.skip.build/go/general/smart-relay` | relay mode, current support statement, fee/expiry and submit/track flow | Smart Relay capability must be versioned separately from route generation |
| SG-11 | `https://docs.skip.build/go/advanced-swapping/understanding-quote-quality-metrics` | slippage, USD estimate and price-impact semantics | USD feeds can be stale/unavailable; quote quality is not realized outcome |
| SG-12 | `https://docs.skip.build/go/general/fee-info` | affiliate, bridge, relayer, Smart Relay and gas fee categories | estimated fee is not necessarily realized total cost |

## Verification status

- Standalone C04 and B01–B04 bytes were hash-verified on `2026-08-29 KST`.
- SG-01–SG-12 are official live-document snapshots reviewed on `2026-08-30`;
  repository byte preservation and hashing have not been authorized or performed
  in this channel session.
- Source refresh is affected-claim-only. Do not restart a whole Skip Go survey
  unless a material implementation or baseline conflict is identified.
