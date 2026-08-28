# COSMOS HUB BM2 — MULTI-PATH / FAILOVER / RECOVERY

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-04

CHANNEL =
COSMOS HUB BM2 — MULTI-PATH / FAILOVER / RECOVERY

PACKET_TYPE =
ROUTE-DIVERSITY / FAILOVER / SPLIT / HEDGED SEPARATION / RECOVERY SAFETY / NO LIVE EXECUTION

DATE_KST =
2026-08-29


SOURCE_DOCUMENT =
COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE

SUPPORTING_DOCUMENTS =
1. 00_OWNER_REVIEW_INDEX.md
2. V1.2_6G_PRIOR_ART_EVIDENCE_LEDGER.md
3. V1.2_6G_CONCEPT_SELECTION_MATRIX.md
4. V1.2_PARALLEL_TRACK_ROADMAP_CANDIDATE.md

SOURCE_STATUS =
STEP 3–5 OWNER-REVIEW CANDIDATE
OVERALL CLASSIFICATION = B. SELECTIVE FIT



OWNER_ACTION_REQUIRED =
FALSE — 본 채널의 부트스트랩·조사·설계 토론은 진행 가능
TRUE — Owner 선택, 공통 경계 변경, 본문 반영, 파일럿·구현 승인이 필요할 때만

PRODUCTION_AUTHORIZED =
FALSE

FULL_V1_2_REWRITE_AUTHORIZED =
FALSE

NEW_BM_AUTHORIZED =
FALSE

NATIVE_MODULE_DESIGN_AUTHORIZED =
FALSE

LIVE_ROUTING_OR_FINANCIAL_EXECUTION_AUTHORIZED =
FALSE

COMMERCIAL_SLA_OR_COMPENSATION_AUTHORIZED =
FALSE

FORMAL_6G_CONFORMITY_CLAIM_AUTHORIZED =
FALSE


NEXT_OWNER_REVIEW =
BM2-MP-06에서 각 메커니즘의 독립 Go/Hold/Kill 선택이 필요할 때


AUTHORITY PRECEDENCE =
1. OWNER의 최신 명시적 결정
2. CH-00 INTEGRATION / OWNER DECISIONS의 최신 통합 결정
3. 본 패킷의 COMMON HARD LOCKS
4. 본 채널의 LOCAL HARD LOCKS와 CHANNEL-SEALED 결정
5. Working Note / 가설 / 초안

DECISION EFFECT =
- 본 채널의 결론은 기본적으로 CANDIDATE이다.
- CH-00 통합과 필요한 Owner 결정 전에는 프로젝트 확정안이 아니다.
- 다른 채널의 범위·권한·객체 정의를 묵시적으로 변경하지 않는다.
- 기존 결정 변경 시 새 Decision ID와 SUPERSEDES를 기록한다.

DECISION LIFECYCLE =
WORKING
→ CANDIDATE
→ CHANNEL-SEALED
→ CH-00 REVIEWED
→ OWNER DECIDED
→ INTEGRATED


DECISION_ID PREFIX =
BM2-MP-D

===============================================================================
0. COMMON GOVERNANCE
===============================================================================


COMMON HARD LOCKS =
- 네 개 BM과 우선순위를 유지한다.
  1) Interchain Asset Distribution Market
  2) Assured Interchain Delivery SLA
  3) Enterprise One-Connection Gateway
  4) Asset & Service Registry
- Thin Core, Rich Edges 원칙을 유지한다.
- Base IBC는 개방형이며 강제 Hub 통행료를 부과하지 않는다.
- Hub는 고객 원금을 보관하지 않는다.
- Hub 자체 DEX·Lending·Perp·Stablecoin·Market Making·독점 Router를 기본안으로 추가하지 않는다.
- ATOM을 강제 결제자산으로 만들지 않는다.
- KYC 원자료·PII·기관의 민감 정책 원문을 public chain에 저장하지 않는다.
- 계약·데이터·작은 audited CosmWasm MVP를 먼저 검증한다.
- Native Module은 반복 운영의 실제 병목이 증명된 뒤 별도 Owner 승인으로만 검토한다.
- AI는 private key를 보관하거나 transaction을 승인하지 않는다.
- AI는 hard policy, exposure cap, minimum receive, finality, allowlist를 임의 변경하지 않는다.
- AI는 보상·분쟁·법적 책임을 단독 판정하지 않는다.
- 전역 atomic revert, 원금보장, 보험, 규제 적합성 보장을 암시하지 않는다.
- 복수 provider 경쟁, open specification, switching 가능성을 유지한다.
- 6G-compliant, 6G-certified, IMT-2030 compliant, 3GPP 6G implemented 표현을 사용하지 않는다.
- 현재 로드맵은 선택적 prior-art 적용안이며 생산 아키텍처 승인이 아니다.



STATUS TAXONOMY =
CURRENT IMPLEMENTATION =
현재 Cosmos / IBC / Skip / Wallet / Indexer 등에 실제 존재하는 기능

EXISTING / PARTIAL =
기능 일부 또는 제한된 범위가 현재 존재

SOURCE-SUPPORTED FACT =
제시된 1차 자료가 직접 지지하는 사실

OFFICIAL ROADMAP / CONTRACTUAL ANNOUNCEMENT =
공식 방향 또는 계약 발표이나 운영·수익 실현과 동일하지 않음

V1.2 CHANNEL CANDIDATE =
본 채널이 제안한 미통합 설계

SELECT-LIMITED RESEARCH ITEM =
Hard Gate 아래에서만 검토하는 제한 후보

WATCH =
후속 증거를 기다리는 독립 연구항목

REJECTED BY GOVERNANCE =
Hard Lock 또는 selection 결과로 제외

OWNER DECISION REQUIRED =
전문 채널이 확정할 수 없는 선택

CH-00 INTEGRATION REQUIRED =
공통 객체·우선순위·타 채널 인터페이스에 영향을 주는 항목


===============================================================================
1. CHANNEL-SPECIFIC GOVERNANCE
===============================================================================


CHANNEL ROLE =
BM2 Route Diversity / Failover / Split / Recovery Safety Channel

PRIMARY QUESTION =
Candidate Route Diversity, Sequential Failover, Split Routing,
Redundant/Hedged Execution 중 무엇이 실제 reliability와 경제성을 개선하며,
어디서 독립적으로 중단해야 하는가?

MISSION =
서로 다른 네 개 메커니즘을 하나의 “multi-path”로 뭉뚱그리지 않고,
각각의 상태머신, duplicate safety, asset-location, recovery, net value를 평가한다.

MANDATORY CLASSIFICATION =
A. Candidate Route Diversity
복수 경로를 계산하고 한 경로를 선택

B. Sequential Failover
실행 전 또는 명시된 안전지점에서 대체 경로로 전환

C. Split Routing
거래액을 여러 leg로 나눠 output/capacity를 최적화

D. Redundant / Hedged Execution
동시에 복수 경로를 사용해 tail/failure risk를 줄이려는 별도 고위험 방식

CURRENT BASELINE =
- Candidate Route Diversity = EXISTING / PARTIAL
- Smart-Swap Split Routing = EXISTING / PARTIAL
- General Sequential Failover = PARTIAL / SELECT-LIMITED
- Redundant / Hedged Execution = WATCH / DEFAULT-OFF

IN SCOPE =
- candidate route set와 route-plan hash
- pre-execution health check
- quote expiry와 route replacement
- authorization 전후의 failover point
- idempotency와 retry
- unique execution ID
- per-leg amount/exposure cap
- duplicate suppression
- leg state와 aggregate completion
- last-known asset location
- partial completion과 stranded intermediate asset
- recovery owner, deadline, capital release
- fee/gas/liquidity/recovery/accounting cost
- route diversity, sequential failover, split, hedge의 독립 PASS/HOLD/KILL
- historical replay와 bounded failure simulation

OUT OF SCOPE =
- AI model 학습·prediction 성능
- SLO와 legal breach의 최종 정의
- provider eligibility와 registry badge
- enterprise service UX
- production multi-path 배포
- 일반적인 “자동 복구” 또는 global atomicity 주장

LOCAL HARD LOCKS =
- 네 메커니즘을 하나의 기능이나 KPI로 합치지 않는다.
- Hedged Execution은 DEFAULT-OFF이며 별도 Owner 승인 없이는 live test하지 않는다.
- exact failover point와 current asset location이 불명확하면 reroute하지 않는다.
- unique execution ID와 duplicate suppression이 없으면 다음 단계로 가지 않는다.
- split/hedge의 각 leg에 독립 receipt와 recovery owner를 둔다.
- aggregate completion rule을 실행 전 고정한다.
- 추가 success benefit만 보지 않고 추가 비용·locked capital·recovery를 차감한다.
- current Smart-Swap 기능을 새로운 Cosmos Hub 기능으로 오표기하지 않는다.
- AI health score는 실행허가가 아니라 입력 신호다.
- mid-flight failover는 pre-execution replacement보다 훨씬 높은 Safety Gate를 요구한다.

MANDATORY INVARIANTS =
unique execution ID
route-plan hash
per-leg amount and exposure cap
leg start / complete / fail state
aggregate completion rule
last-known asset location
duplicate suppression
recovery owner and deadline
capital-release rule
compensation reference

NET ROUTE VALUE =
Incremental Success / Output / Tail-Latency Benefit
- Extra Provider Fee
- Extra Gas
- Liquidity / Price Impact
- Recovery and Support Cost
- Locked-Capital Cost
- Compliance / Accounting Overhead
= Net Route Value

ORDERED EVALUATION =
1. Existing candidate route diversity를 baseline으로 기록
2. 실행 전 provider/client/channel health check
3. authorization 전 deterministic route replacement
4. idempotency가 증명된 범위의 bounded retry
5. per-leg receipt가 있는 split evaluation
6. Hedged Execution은 별도 연구로 유지

DEPENDENCIES =
INPUT FROM CH-02 =
time, leg, failure, recovery, last-known-location evidence semantics

INPUT FROM CH-03 =
advisory route risk/health estimates와 confidence

INPUT FROM CH-06 =
provider capability, route support, incident history

INPUT FROM CH-07 =
duplicate liability, partial-leg accounting, exposure and compensation boundary

OUTPUT TO CH-05 =
사용자·기관에 공개할 route/failover/split/recovery 조건

OUTPUT TO CH-00 =
각 메커니즘별 독립 promotion/kill 결정

REQUIRED OUTPUTS =
BM2-MP-01 = MULTIPATH_TAXONOMY_AND_EXISTING_BASELINE
BM2-MP-02 = ROUTE_PLAN_LEG_AND_STATE_MACHINE
BM2-MP-03 = IDEMPOTENCY_DUPLICATE_SUPPRESSION_INVARIANTS
BM2-MP-04 = RECOVERY_ASSET_LOCATION_AND_CAPITAL_RELEASE_MODEL
BM2-MP-05 = NET_ROUTE_VALUE_ASSESSMENT
BM2-MP-06 = INDEPENDENT_GO_HOLD_KILL_DECISIONS

PASS — ROUTE DIVERSITY =
후보 경로의 trust, liquidity, health 차이를 사실적으로 비교할 수 있다.

PASS — SEQUENTIAL FAILOVER =
- failover point가 명확하다.
- duplicate execution이 없다.
- quote·minimum receive·policy를 다시 검증한다.
- last-known asset location과 recovery가 재현된다.
- net value가 양수다.

PASS — SPLIT =
- per-leg evidence와 aggregate completion이 명확하다.
- partial failure recovery가 가능하다.
- realized output 개선이 추가 비용보다 크다.

PASS — HEDGE =
기본적으로 없음.
duplicate settlement 방지, accounting/legal, capital release, net value가 모두 별도 증명된 경우에만 Candidate로 재심사한다.

HOLD =
- narrow route에서만 benefit이 있다.
- per-leg evidence 또는 idempotency가 불완전하다.
- asset location이나 recovery owner가 불명확하다.

KILL =
- duplicate execution 또는 stranded asset 위험이 남는다.
- multi-path가 recovery와 accounting을 악화시킨다.
- net route value가 음수다.
- 안전을 위해 global custody나 Hub 독점 실행이 필요하다.

CURRENT START POINT =
BM2-MP-01에서 existing/partial/new를 고정하고,
BM2-MP-02~04 없이는 구현 논의를 시작하지 않는다.


===============================================================================
2. VALIDATION / HANDOFF / REPORTING
===============================================================================


VALIDATION POLICY =
- 수정된 주장, 변경된 객체, 영향받은 인터페이스만 검증한다.
- 전면 재조사·전역 regression·반복 validation loop를 만들지 않는다.
- 사실, 제안, 추론, 미검증 가설을 구분한다.
- 필요한 주장에는 SOURCE CLASS, IMPLEMENTATION STATUS, CLAIM CEILING을 붙인다.
- 증거가 없으면 UNKNOWN 또는 HOLD로 기록하고 추정으로 메우지 않는다.
- PASS는 정확한 문서·스키마·데이터·코드·계약 범위에 바인딩한다.
- 선택 트랙 하나의 FAIL이 관련 없는 다른 트랙을 자동 무효화하지 않는다.

CLAIM CEILING =
C0 = 내부 가설
C1 = 구조적 정렬
C2 = 공식 연구를 참조한 선택적 설계
C3 = 측정된 bounded PoC
C4 = 범위가 공개된 운영 파일럿
C5 = 정식 적합성평가 이후만 가능

CURRENT MAXIMUM =
C2 — PoC 전



CHANNEL → CH-00 HANDOFF FORMAT =
FROM_CHANNEL =
DECISION_ID =
STATUS =
QUESTION =
RECOMMENDED_DECISION =
ALTERNATIVES_CONSIDERED =
EVIDENCE =
RATIONALE =
IMPACTED_CHANNELS =
IMPACTED_BM =
IMPACTED_TRACK =
HARD_LOCK_CHECK =
DEPENDENCIES =
LEGAL_SAFETY_ECONOMIC_EFFECT =
CLAIM_CEILING =
OWNER_ACTION_REQUIRED =
PROPOSED_INTEGRATION =
SUPERSEDES =

HANDOFF RULE =
- 서술형 요약만 보내지 않는다.
- 결정·근거·영향·미해결점을 분리한다.
- 다른 채널이 필요한 경우 CH-00이 의존성을 등록한다.
- 반복적인 수동 재설명 대신 Decision ID를 공통 참조점으로 사용한다.



CHANNEL REPORT FORMAT =
OVERALL_PROGRESS =
CURRENT_WORKSTREAM =
CURRENT_QUESTION =
CURRENT_BASELINE =
MATERIAL_FINDINGS =
DECISION_CANDIDATES =
ALTERNATIVES =
DEPENDENCIES =
RISKS =
BLOCKERS =
OWNER_ACTION_REQUIRED =
NEXT_STEP =


END PACKET
