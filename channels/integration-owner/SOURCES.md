# CH-00 Sources

Exact canonical repository paths are used so the source-ingest lane can preserve bytes independently. Raw sources outrank this derived channel memory.

| ID | Canonical repository path | SHA-256 | Status / authority | Use and caution |
|---|---|---|---|---|
| C01 | `sources/raw/channel-policy-packets/v1.0/00_CH00_INTEGRATION_OWNER_DECISIONS_PACKET.md` | `1364b6e649a91d8c1449cc709e0dbcf6cc462ccc92f110520622207d5f082eb8` | Exact standalone channel policy packet | Controlling charter input; use this corrected standalone hash, not an older archive copy |
| A01 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.docx` | `19f948efcc43987213bb5f71157dd17ac98fb1a88e5acc2b474bd1cc1a966610` | Candidate; independent proposal; not official Hub policy | Proposal baseline; no production or governance authority |
| A02 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.pdf` | `d71c4dea192db1facde65fce5dbc164d8586bc386438253b0b4126a13a99622b` | Rendered Candidate companion | Presentation copy; raw DOCX/text and source status remain controlling |
| A03 | `sources/raw/v1.1/Cosmos_Hub_BM_Improvement_Proposal_v1.1_CANDIDATE.txt` | `b298db88356148798f57be5f8ea4335959c3e79d499860bd2fd81dc3f8545105` | Candidate text companion | Searchable baseline; not official policy |
| B01 | `sources/raw/v1.2-step3-5/00_OWNER_REVIEW_INDEX.md` | `c70dfbc6a4686be23fdf1b56ce32f57c3fdf538dde147e704044894d1b5a5bd1` | Owner-review Candidate | Index/decision summary only; does not evidence Owner approval |
| B02 | `sources/raw/v1.2-step3-5/V1.2_6G_PRIOR_ART_EVIDENCE_LEDGER.md` | `1e4397684d8c8fabc139b9a47843066a2c142ec0da277c6d7199c3f0a656f75a` | Owner-review Candidate | Evidence ledger; selective prior-art only, no conformity claim |
| B03 | `sources/raw/v1.2-step3-5/V1.2_6G_CONCEPT_SELECTION_MATRIX.md` | `b4c0829a71726cea5997ebd7927863979f1c34178cab51acae9e807155565dfc` | Owner-review Candidate | Candidate scoring/selection; `SELECT` is not Owner-decided |
| B04 | `sources/raw/v1.2-step3-5/V1.2_PARALLEL_TRACK_ROADMAP_CANDIDATE.md` | `e7455c86a0382b846a8cd5034ea2215068217231beebb0eded7b63ff3e9026bc` | Owner-review Candidate | Roadmap/OR recommendations; no implementation or rewrite authority |

Source verification snapshot: standalone C01 and current B01–B04 bytes were hash-verified on `2026-08-29 KST`. Source publication, manifest, and byte preservation remain the source-ingest lane's responsibility.
