# BM2-AI-01 — Current Skip Go Functional Baseline (Draft)

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
CHANNEL = CH-03 — AI-ASSISTED SKIP GO ROUTING
DELIVERABLE = BM2-AI-01
TOPIC = T02 — CURRENT SKIP GO FUNCTIONAL BASELINE
STATUS = SOURCE-GROUNDED DRAFT / NOT FROZEN
SOURCE_SNAPSHOT = 2026-08-30
MODEL_SELECTED = FALSE
LIVE_ROUTING_AUTHORIZED = FALSE
CLAIM_CEILING = C2 MAXIMUM
```

This draft documents current Skip Go behavior before any AI model, comparator
freeze, route-universe choice or improvement claim. Current routing, candidate
route diversity and Smart-Swap splitting remain existing/partial capabilities,
not new AI or 6G inventions.

## 1. Plain-language baseline

Skip Go is an off-chain interoperability and routing service, not a blockchain,
not the Cosmos Hub, and not a user wallet. It combines a route/quote engine,
asset and chain information, DEX/bridge composition, transaction-message
construction, optional relay services and transaction tracking.

The normal product flow is:

```text
chain/asset information
→ route and quote
→ user-controlled addresses
→ transaction/message construction
→ user signing
→ submission or tracking registration
→ multi-hop status and failure observation
```

Skip Go can recommend and compose operations, but the user or institution still
supplies signing authority. Chain, bridge, DEX and relayer mechanisms perform the
actual asset movement and state transition.

## 2. Current service boundary

### 2.1 Supported integration surfaces

Official documentation exposes three integration levels:

1. REST endpoints for maximum control;
2. the actively maintained `@skip-go/client` TypeScript package;
3. an embeddable widget.

The high-level platform composes swaps and transfers across Cosmos, EVM and SVM
ecosystems using underlying DEXes and messaging/bridge protocols. Current route
request bridge enums include IBC, Axelar, CCTP, Hyperlane, OP Init, Go Fast,
Stargate, LayerZero and Eureka. Availability remains route-, asset-, chain- and
configuration-dependent.

### 2.2 Principal API flow

```text
GET  /v2/info/*
POST /v2/fungible/route
POST /v2/fungible/msgs
POST /v2/fungible/msgs_direct
POST /v2/tx/submit   OR   POST /v2/tx/track
GET  /v2/tx/status
```

- `/route` returns a route, quote and operation sequence.
- `/msgs` converts an already selected route into transaction data.
- `/msgs_direct` combines route/quote and message construction.
- `/submit` broadcasts through Skip infrastructure and registers tracking.
- `/track` registers an externally submitted transaction for tracking.
- `/status` reports overall and per-transfer progress.

### 2.3 Route request controls

Current documented controls include:

```text
source_asset_denom
source_asset_chain_id
dest_asset_denom
dest_asset_chain_id
amount_in OR amount_out
cumulative_affiliate_fee_bps
swap_venues[]
allow_unsafe
experimental_features[]
allow_multi_tx
bridges[]
smart_relay
smart_swap_options
allow_swaps
go_fast
```

Because these flags alter the candidate universe, a valid comparator must store
the complete request rather than only source, destination and amount.

### 2.4 Route response surface

Documented route responses can include:

```text
amount_in / amount_out
source and destination chain/denom
operations[]
operation tx_index
chain_ids[]
required_chain_addresses[]
does_swap
estimated_amount_out
swap venue(s)
txs_required
usd_amount_in / usd_amount_out
swap_price_impact_percent
estimated_fees[]
estimated_route_duration_seconds
```

`operations[]` is the current observable representation of transfers, swaps and
bridge-specific legs. It is useful as an input to the later CH-03 route/leg
schema, but it is not yet the frozen BM2 canonical representation.

## 3. IBC token-denom/path algorithm is a sub-baseline

The official IBC routing document describes a narrow but important algorithm:

1. unwind the asset back toward its origin chain;
2. apply any high-priority manual override for the asset/destination pair;
3. otherwise select the most liquid direct IBC path from origin to destination;
4. return no recommendation when there is no direct path, the relevant client is
   expired, or the asset has never used that direct path.

The service indexes supported-chain client/channel state and token liquidity on
a recurring basis. The official page describes these refreshes as occurring
every few hours, so a later rerun is not guaranteed to reproduce a historical
route without a captured request/response snapshot.

This IBC denom-recommendation logic must not be confused with the complete Skip
Go cross-ecosystem route-composition engine. The wider API can combine transfer,
bridge and swap operations across multiple protocols.

## 4. Existing swap and route-diversity functions

Smart Swap currently documents:

- comparison of Skip's in-house router and supported external routers;
- route splitting across multiple swap paths/pools for price execution;
- EVM swap support.

A split route may return multiple swap routes and operations. This is existing or
partial product behavior and becomes an evaluation baseline. It is not evidence
that redundant cross-chain asset execution, generalized failover or an AI router
is already safe.

## 5. Transaction construction and authorization boundary

`/msgs` and `/msgs_direct` return messages or transaction data, a route and a
minimum amount out. The client `executeRoute` helper validates required
addresses, checks gas conditions, can simulate transactions and executes the
sequence across Cosmos, EVM and SVM using signer functions supplied by the
integrator/user.

Therefore:

```text
Skip route recommendation ≠ transaction authorization
Skip message construction  ≠ private-key custody
Skip tracking              ≠ independent commercial adjudication
```

Every `required_chain_address` should be user-controlled. Official guidance
warns that funds can remain at an intermediate address under certain failures.

## 6. Submission, relay and tracking

A signed transaction may be submitted through `/submit`, or independently
broadcast and then registered through `/track`. `/status` exposes an overall
state, a transfer sequence, the next blocking transfer where applicable, asset
release information and errors.

Documented terminal top-level states include:

```text
STATE_COMPLETED_SUCCESS
STATE_COMPLETED_ERROR
STATE_ABANDONED
```

Non-terminal states are interpreted as pending/in progress. Per-leg errors must
be inspected because a terminal overall error may not retain a non-null
`next_blocking_transfer`.

Smart Relay is a separate Skip delivery service. The route API documents the
`smart_relay` switch, while the current Smart Relay page states that CCTP is
supported and IBC, Hyperlane and Axelar support is being built. Unsupported
bridges continue to use public or enshrined relayers. This capability must be
versioned separately from the route engine in any comparator.

## 7. Current failure and recovery behavior

### 7.1 IBC pre-swap or swap failure

Typical causes include packet timeout, slippage, invalid recovery address and an
expired IBC client. The documented IBC outcome is return of the original source
asset to the starting source-chain address.

### 7.2 IBC post-swap failure

After a swap succeeds but a later transfer fails, the purchased destination
asset can be released to the user's address on the swap chain.

### 7.3 Multi-transaction caveat

For a multi-transaction route, it is not generally correct to say assets always
return to the original source or swap chain. A failure can leave assets on the
chain targeted by the last successfully initiated transaction. This is why
last-known asset location and user-controlled intermediate addresses are
mandatory BM2 evidence fields.

### 7.4 Protocol-specific differences

- Axelar failure recovery can differ from IBC and may leave the bridged token on
  the intended swap chain.
- A CCTP attestation outage can leave source-burned funds inaccessible until the
  attestation service recovers.
- Hyperlane delivery depends on the route's configured ISM requirements.
- Go Fast documents timeout-driven refund behavior.

The current product therefore provides protocol-specific status and recovery
behavior, not one global atomic rollback or principal guarantee.

## 8. What the official sources do not yet establish

The reviewed public documentation does not by itself establish:

- the complete proprietary scoring function across all route candidates;
- a versioned historical candidate set for counterfactual replay;
- complete historical feature/label access for every route and failed leg;
- independent commercial-SLA adjudication;
- a generalized provider-health probability model;
- safe arbitrary mid-flight rerouting;
- a production AI route-optimization layer;
- a route outcome guarantee.

Record these as `UNKNOWN`, `PARTIAL` or later data-readiness questions rather
than infer them.

## 9. Candidate baseline-freeze design

One baseline is insufficient because product defaults can change. CH-03 should
retain two related Skip baselines:

```text
B0-A SKIP_DEFAULT_AS_SERVED
= exact request with product defaults as served at a recorded timestamp

B0-B SKIP_EXPLICIT_FROZEN_CONFIG
= the same route universe with every material flag explicitly stored
```

Each observation should bind at least:

```text
request_id
request_timestamp
endpoint
complete request body
API/client version where available
API-key/access tier where material
route response bytes/hash
candidate operations and tx_index
quote/relay-fee expiry
estimated output, fees, price impact and duration
required addresses and tx count
registry/source snapshot references where available
subsequent tracking identifier
realized completion/failure/recovery evidence
```

`B0-A` measures the current product experience. `B0-B` improves reproducibility.
Neither is frozen until T03 route representation and T04 comparator rules close.

## 10. Status distinction

```text
CURRENT IMPLEMENTATION = route/quote, multi-protocol composition, message
construction, user-signer client execution, submit/track/status, existing Smart
Swap and protocol-specific failure handling

SOURCE-SUPPORTED = the official documentation behavior summarized above

UNKNOWN / RESEARCH-OPEN = complete route-scoring internals, historical candidate
sets, data/label coverage, independent adjudication and generalized failover

CHANNEL CANDIDATE = dual Skip baseline B0-A/B0-B and the required snapshot fields

NOT AUTHORIZED = model selection, live AI authority, production routing,
commercial SLA, native module or v1.2 promotion
```

## 11. Official source set reviewed

- https://docs.skip.build/go/general/getting-started
- https://docs.skip.build/go/general/overview-and-typical-usage
- https://docs.skip.build/go/api-reference/prod/fungible/post-v2fungibleroute
- https://docs.skip.build/go/api-reference/prod/fungible/post-v2fungiblemsgs_direct
- https://docs.skip.build/go/advanced-transfer/ibc-routing-algorithm
- https://docs.skip.build/go/advanced-swapping/smart-swap-options
- https://docs.skip.build/go/client/executing-a-route
- https://docs.skip.build/go/advanced-transfer/interpreting-transaction-status
- https://docs.skip.build/go/advanced-transfer/handling-cross-chain-failure-cases
- https://docs.skip.build/go/general/smart-relay
- https://docs.skip.build/go/advanced-swapping/understanding-quote-quality-metrics
- https://docs.skip.build/go/general/fee-info

## 12. Remaining closure questions for T02

1. Is there a public, versioned route-engine or registry release identifier that
   can be bound to every observation?
2. Which documented defaults vary by endpoint/client version or access tier?
3. Can the API expose the complete candidate set, or only the selected route?
4. What historical route, quote, status and failure data are accessible under a
   reproducible research agreement?
5. Which Smart Relay capabilities were active for each historical observation?
6. Which status fields can be independently corroborated from chain/protocol
   evidence?

Until these close, T02 is `DRAFTED / NOT FROZEN`.
