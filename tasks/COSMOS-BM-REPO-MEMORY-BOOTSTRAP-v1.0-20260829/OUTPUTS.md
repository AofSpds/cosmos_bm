# Task Outputs — Validated D0 / PR-Ready Index

This index records the bounded bootstrap Candidate outputs. Exact completion,
validation, PR/merge, and post-merge evidence are added only when they exist.

## Current outputs

| Output | Path or exact ref | Current state |
|---|---|---|
| Genesis/base | `a3b18e231e5e3c7c053d3a838e4047ea218e4aa2` | created/read back |
| Governance core lane | `63a3afb267d2dace3d28a945f903c5ef4d7e6e51` | Candidate lane merged |
| Source ingest lane | `62945dbfeecb5dc37530870092890c7ef1651d2f` | 26/26 allowlisted; 0 missing |
| CH-00–CH-03 lane | `05467f1592432ec8367c58c51a4db9ea9a061ae2` | four seven-file channel sets |
| CH-04–CH-07 lane | `85461bb61f5434da866df2565524e1e2c6664b18` | four seven-file channel sets |
| Ordered lane merge | `f482e23980d91d04a26e83e25157dc9966f4cf7a` | local/remote tree matched |
| Validated D0 | `7de27f727582c4626c76728fbdf4196b40007591` | independent PASS; exact target only |
| D0 tree | `b8efa3947db1fd6d0b89c6c2fcf200775a0c5242` | clean target reconfirmed |
| Current pointer | `COSMOS_BM_BOOTSTRAP_CURRENT.json` | validated Candidate / PR pending |
| Governance | `governance/v1.0/` | validated Candidate / no semantic promotion |
| Channel current sets | `channels/*/` | 8 × 7 core files |
| Source manifest/checksums | `sources/SOURCE_MANIFEST.yaml`, `sources/SHA256SUMS.txt` | 26 imports recorded |
| Structural checks | `STRUCTURAL_CHECKS.md` | S01–S18 PASS on final pre-D0 tree |
| Validation receipt | `validation/VALIDATION_RECEIPT.md` | PASS; SHA-256 `05b5547d4ffa7ff8616d42a4b411baa96c829c47bff00c4b30fd025fcd2df3f7` |

## Explicitly absent at this checkpoint

- D1 (not required because there was no correction)
- main PR/merge and post-merge readback
- Owner acceptance or activation

No absence above is silently inferred as a decision. Validation does not
transfer from D0 to later administrative metadata.
