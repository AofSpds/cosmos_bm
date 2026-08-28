# CH-02 Open Questions

All questions remain open Candidate-design questions. No Owner decision, commercial SLA, or compensation authority is inferred.

## Completion, time, and finality

- Which exact event proves completion for each bounded route class?
- What chain-specific profile defines `agreed finality reached`?
- Which timestamp source and clock semantics govern quote, authorization, inclusion, finality, leg, failure, recovery, and compensation time?
- What freshness thresholds make evidence stale rather than current?

## Failure, recovery, and evidence

- How are provider-controlled failure, user error, chain halt, bridge halt, and exempt external event classified reproducibly?
- When is last-known asset location sufficiently evidenced?
- Which missingness forces `HOLD` or `UNRESOLVED` rather than success/breach?
- How are conflicts among chain state, packet/bridge state, independent indexers, and provider-signed telemetry reconciled?
- What evidence completeness is required for each preserved Recovery State?
- What minimum receipt is public/on-chain, and what detailed evidence remains off-chain to preserve privacy?

## SLO/SLA boundary

- Which metrics belong in the Interchain SLO dictionary?
- Which subset alone could be objectively contracted in an explicitly authorized bounded M3 pilot?
- Which exception and controllability rules separate an SLO miss from a commercial breach?
- What evidence supports a dispute without making one provider or indexer sole adjudicator?
- Which CH-01/03/04/05/06/07 inputs must be fixed before channel seal?

Owner action is not required for bounded evidence design. It becomes required for M1/M3 scope selection, commercial SLA/compensation, pilot, live execution, implementation, text integration, or another separately controlled approval.
