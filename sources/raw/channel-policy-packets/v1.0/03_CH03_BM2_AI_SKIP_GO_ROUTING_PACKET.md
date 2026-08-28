# COSMOS HUB BM2 — AI-ASSISTED SKIP GO ROUTING

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-03

CHANNEL =
COSMOS HUB BM2 — AI-ASSISTED SKIP GO ROUTING

PACKET_TYPE =
AI ROUTING RESEARCH / DETERMINISTIC BASELINE / SHADOW MODE / NO LIVE AUTHORITY

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
Shadow 평가계획 또는 BM2-AI-06 Promotion/Hold/Kill 선택이 필요할 때


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
BM2-AI-D

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
AI-assisted Routing Research / Deterministic Baseline Comparison Channel

PRIMARY QUESTION =
AI 예측이 현재 Skip Go와 규칙 기반 deterministic routing보다
실제 realized outcome을 재현 가능하게 개선하는가?

MISSION =
AI 도입을 전제로 하지 않는다.
현재 Skip Go 기능을 정확한 baseline으로 고정하고,
M2 Shadow Mode에서 prediction·calibration·drift·net value를 검증한다.

IN SCOPE =
- 현재 Skip Go route API와 routing algorithm
- candidate route 생성, quote refresh, liquidity·slippage
- current route diversity와 Smart-Swap split 기능의 existing baseline
- route-time feature와 label availability
- latency distribution prediction
- realized output / slippage prediction
- failure probability
- recovery probability와 expected recovery time
- provider anomaly / health signal
- risk-adjusted candidate scoring
- deterministic optimizer interface
- confidence, calibration, abstention, drift, rollback
- model version binding과 feature timestamp
- shadow evaluation과 adversarial test
- added API/compute/ops cost

OUT OF SCOPE =
- private key, signature, transaction authorization
- live policy mutation
- bridge/asset/provider allowlist 변경
- exposure cap, minimum receive, finality 완화
- compensation·breach 최종 판정
- multi-path execution state machine
- provider factual eligibility의 최종 결정
- Hub-owned proprietary mandatory router
- production inference authorization

LOCAL HARD LOCKS =
- AI는 prediction과 advisory ranking까지만 담당한다.
- deterministic optimizer와 hard policy engine이 authoritative하다.
- wallet 또는 institution authorization을 유지한다.
- confidence 부족 시 abstain하고 frozen baseline으로 fallback한다.
- current Skip Go route를 신규 6G 기능으로 재포장하지 않는다.
- Smart-Swap split routing을 AI 신규 발명으로 주장하지 않는다.
- future information leakage가 있는 feature를 사용하지 않는다.
- provider rank와 eligibility를 분리한다.
- model output에 version, feature time, confidence, abstention을 바인딩한다.
- M2 Shadow 결과 없이 live routing 개선을 주장하지 않는다.
- 평균 개선만으로 승격하지 않고 p95/p99, 실패, recovery, cost를 함께 본다.

MANDATORY DETERMINISTIC COMPARATORS =
Current Skip Go / Default Route
Shortest Path
Lowest Quoted Cost
Maximum Quoted Output
Minimum Hop
Rule-based Weighted Score

ALLOWED MODEL OUTPUTS =
Completion-time distribution
Realized-output / slippage estimate
Failure probability
Recovery probability
Expected recovery duration
Provider health / anomaly signal
Risk-adjusted candidate score
Human-readable explanation draft

PROHIBITED MODEL OUTPUT EFFECT =
Direct transaction approval
Private-key use
Unregistered provider addition
Hard-policy override
Exposure increase
Minimum-receive reduction
Finality weakening
Compensation decision
Silent route mutation after authorization

DEPENDENCIES =
INPUT FROM CH-02 =
frozen feature/label definitions, timestamps, provenance, recovery states

INPUT FROM CH-04 =
route candidate and leg representation; failover/split classification

INPUT FROM CH-06 =
factual capability, provider identity, evidence freshness

INPUT FROM CH-07 =
model responsibility, bias, concentration, economic and claim boundaries

OUTPUT TO CH-04 =
route risk estimates는 advisory input일 뿐 실행허가가 아님

OUTPUT TO CH-05 =
structured intent에 표시할 예측값·confidence·explanation schema

OUTPUT TO CH-00 =
AI promotion, HOLD, permanent Shadow, KILL 결정

REQUIRED OUTPUTS =
BM2-AI-01 = CURRENT_SKIP_GO_AND_DETERMINISTIC_BASELINE
BM2-AI-02 = FEATURE_LABEL_AND_DATA_READINESS
BM2-AI-03 = SHADOW_EVALUATION_PROTOCOL
BM2-AI-04 = CALIBRATION_DRIFT_ABSTENTION_MODEL_GOVERNANCE
BM2-AI-05 = BASELINE_COMPARISON_AND_NET_VALUE_REPORT
BM2-AI-06 = PROMOTION_HOLD_KILL_RECOMMENDATION

EVALUATION REQUIREMENTS =
- dataset split와 route universe를 사전 고정한다.
- feature는 quote/decision 시점에 이용 가능해야 한다.
- applicable baseline을 모두 비교한다.
- ranking accuracy뿐 아니라 probability calibration을 본다.
- stale/missing data, provider outage, chain halt, price movement, drift를 시험한다.
- abstention과 fallback 성공률을 측정한다.
- compute/API latency와 운영비를 포함한다.
- asset, chain, provider, market regime별 성능을 분리한다.

PASS =
- out-of-sample에서 reproducible improvement가 있다.
- calibration과 tail error가 허용범위다.
- confidence 부족 시 안전하게 abstain/fallback한다.
- added cost를 제외한 net route value가 양수다.
- provider concentration과 discrimination 위험을 통제할 수 있다.

HOLD =
- label이 희소하거나 특정 route에만 개선된다.
- drift와 calibration이 불안정하다.
- data freshness 또는 source dependence가 과도하다.

KILL / PERMANENT SHADOW =
- deterministic baseline 대비 material gain이 없다.
- 안전한 abstention/fallback이 불가능하다.
- 모델 이득보다 API·compute·운영비가 크다.
- ranking이 provider 독점 feedback을 통제 불가능하게 강화한다.
- live use를 위해 Hard Lock 변경이 필요하다.

CLAIM RULE =
M2 = “shadow evaluated” C2
Measured bounded PoC = C3
“AI-optimized production routing”은 운영 파일럿 전 사용 금지

CURRENT START POINT =
BM2-AI-01과 BM2-AI-02를 먼저 닫고 모델 선택은 후행한다.


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
