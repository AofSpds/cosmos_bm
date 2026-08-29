# CH-03 Current Memory

> Compact current-state summary. It is not a transcript and does not outrank
> Git-persisted Owner decisions, `CHANNEL.md`, `DECISIONS.jsonl`, or exact
> sources.

## Identity

- Channel: `CH-03 — AI-ASSISTED SKIP GO ROUTING`
- Slug: `ai-assisted-skip-go-routing`
- Decision prefix: `BM2-AI-D`
- Snapshot: `2026-08-30`
- Detailed durable topic map: `TOPIC_INDEX.md`
- Active deliverable draft: `BM2-AI-01_CURRENT_SKIP_GO_BASELINE_DRAFT.md`

## Current state

- v1.1 proposal: `CANDIDATE`, independent and non-official.
- STEP 3–5 package: `OWNER-REVIEW CANDIDATE`.
- Overall classification: `B. SELECTIVE FIT — CANDIDATE`.
- Bounded AI-assisted Control Loop and Predictive Assurance / Provider Health:
  `SELECT-LIMITED — CANDIDATE`.
- Candidate Route Diversity and Smart-Swap Split Routing:
  `EXISTING / ASSESS`, not new AI/6G features.
- AI is prediction/advisory only; deterministic optimizer + hard policy +
  explicit wallet/institution authorization remain authoritative.
- M2 Shadow evaluation is required before any promotion claim. No live or
  production inference is authorized.
- Model selection and deployment have not started.
- The decision ledger contains source-derived `BM2-AI-D-0001` plus the exact
  Owner-directed CH-03 discussion/memory protocol `BM2-AI-D-0002`. Neither
  decision seals the channel or authorizes implementation.

## Owner-directed discussion and memory protocol

For every substantive CH-03 response:

1. explain the selected item in plain language;
2. provide the technical/hardcore treatment;
3. distinguish implementation, evidence, inference and proposal;
4. tag `[OWNER-LOCK]`, `[OWNER-DECIDED]`, `[OWNER-QUESTION]`,
   `[OWNER-DECISION-LATER]`, `[CHANNEL-CANDIDATE]`, `[RESEARCH-OPEN]` and
   cross-channel dependencies as applicable;
5. append the compact cumulative CH-03 index at the response bottom.

The footer records the current topic, topic status, BM2-AI-01–06 progress, Owner
decisions, Owner questions, dependencies, memory-update requirement and next
exact topic. Material discussion must be reflected in this memory, the
append-only worklog, decision ledger where applicable, open questions and the
regenerated handoff.

## Fixed safety boundary

AI may output distributions/estimates/probabilities, provider-health signals,
risk-adjusted scores and explanation drafts. It may not approve transactions,
use keys, add providers, override policy, increase exposure, reduce minimum
receive, weaken finality, decide compensation, or silently mutate a route after
authorization. Low confidence requires abstention and fallback to a frozen
deterministic baseline.

## Fixed programme frame

BM order remains Distribution, Assured Delivery, Enterprise Gateway, Registry.
BM1 does not depend on AI. Preserve `Thin Core, Rich Edges`; open untolled base
IBC; no Hub custody, mandatory ATOM, Hub DEX/bridge/stablecoin/lending/perp/
market-making/proprietary mandatory router, public raw KYC/PII/sensitive policy,
unauthorized native module, global atomic revert/principal guarantee/insurance/
regulatory-fitness/formal 6G claim. Preserve provider competition, open
specification and switching.

## Topic map

`TOPIC_INDEX.md` divides the channel into 24 durable topics:

1. mission and authority boundary;
2. current Skip Go baseline;
3. route universe and candidate representation;
4. deterministic comparator suite;
5. objective function and trade-offs;
6. evidence and provenance;
7. time/finality semantics;
8. feature dictionary;
9. label/outcome taxonomy;
10. data readiness and leakage control;
11. dataset split and route-universe freeze;
12. prediction output contracts;
13. model hypotheses without selection;
14. deterministic optimizer and hard-policy interface;
15. calibration and uncertainty;
16. abstention and fallback;
17. Shadow evaluation;
18. drift, robustness and adversarial tests;
19. provider health, neutrality and concentration;
20. provider conflict arbitration;
21. existing route diversity and Smart-Swap split;
22. sequential failover boundary;
23. net route value and operating economics;
24. Promotion/Permanent Shadow/Hold/Kill, claims and CH-00 integration.

## T02 current Skip Go baseline — material findings

- T02 is `SOURCE-GROUNDED DRAFT / NOT FROZEN`.
- Skip Go is an off-chain interoperability/routing service rather than the
  Cosmos Hub, a blockchain or a user wallet.
- Its current documented product flow covers chain/asset information,
  route/quote, transaction-message generation, user-signing integration,
  submission/tracking and multi-hop status observation.
- The narrow IBC denom/path algorithm unwinds to asset origin, applies manual
  overrides, otherwise recommends the most liquid direct IBC path, and returns
  no recommendation when required direct-path conditions fail.
- That IBC algorithm is only one sub-baseline. The wider route API composes
  bridge, transfer and swap operations across multiple ecosystems/protocols.
- Smart Swap external-router comparison and split routing are existing/partial
  functions and remain assessment baselines, not AI novelty.
- Current status/failure semantics are protocol- and leg-specific. Multi-tx
  failures can leave assets on an intermediate transaction-target chain, so
  user-controlled intermediate addresses and last-known asset location are
  mandatory evidence requirements.
- Skip route/message construction does not create transaction authorization,
  private-key custody, independent SLA adjudication, global atomic rollback or a
  route outcome guarantee.
- Candidate baseline design now distinguishes `B0-A SKIP_DEFAULT_AS_SERVED`
  from `B0-B SKIP_EXPLICIT_FROZEN_CONFIG`; neither is frozen before T03/T04.
- Public documentation does not establish the complete proprietary scoring
  function, complete historical candidate sets, historical label coverage,
  generalized provider-health probability models or safe arbitrary mid-flight
  rerouting.

## Active work and progress

- `BM2-AI-01`: `ACTIVE` — T02 drafted from current official documentation;
  T03 route/candidate representation, T04 comparator freeze and T05 objective
  trade-off remain open.
- `BM2-AI-02`: `NOT STARTED` — enumerate features, labels, timestamps,
  provenance, freshness, missingness and leakage controls.
- `BM2-AI-03`: `BLOCKED BY AI-01/02` — Shadow evaluation protocol.
- `BM2-AI-04`: `BLOCKED BY AI-02/03` — calibration, drift, abstention and model
  governance.
- `BM2-AI-05`: `BLOCKED BY AI-03/04` — baseline comparison and net-value report.
- `BM2-AI-06`: `BLOCKED BY AI-05` — Promotion/Permanent Shadow/Hold/Kill
  recommendation.

## Owner questions and timing

No immediate Owner answer is required to continue `BM2-AI-01` or begin
`BM2-AI-02`. Deferred questions are maintained in `TOPIC_INDEX.md` and
`OPEN_QUESTIONS.md`: service-objective trade-off, bounded route universe,
data-readiness threshold, calibration/tail threshold, abstention/fallback
strictness, provider concentration/newcomer policy, added-cost/net-value hurdle,
final Promotion/Hold/Kill choice and public claim/document placement.

## Next gate

- Next exact action: T03 route universe/candidate representation, then T04
  comparator freeze and T05 Pareto/objective analysis to close `BM2-AI-01`.
- Next Owner review: when the Shadow protocol or `BM2-AI-06` recommendation is
  ready, or earlier only if an activated deferred Owner question blocks work.
- Current maximum claim ceiling: `C2 — shadow/research, pre-PoC`.
- Full rewrite, production, live routing/financial execution, commercial
  SLA/compensation, native module, fifth BM and formal 6G claim remain
  unauthorized.
