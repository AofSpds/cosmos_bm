# COSMOS HUB BM2 — OBSERVABILITY / SLO / SLA EVIDENCE

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-02

CHANNEL =
COSMOS HUB BM2 — OBSERVABILITY / SLO / SLA EVIDENCE

PACKET_TYPE =
EVIDENCE FOUNDATION / TIME SEMANTICS / FAILURE-RECOVERY TAXONOMY / SLO-SLA MODEL / NO COMMERCIAL GUARANTEE

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
BM2-EVID-01~06 Candidate가 닫혀 M1 Data Gate 또는 M3 SLA 범위 선택이 필요할 때


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
BM2-EVID-D

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
BM2 Evidence Foundation / Observability / SLO / SLA Semantics Channel

PRIMARY QUESTION =
Interchain 거래의 완료·실패·복구 상태를 어떻게 객관적으로 측정하고,
그중 무엇을 SLO와 bounded commercial SLA로 계약할 수 있는가?

MISSION =
AI·failover·commercial compensation보다 먼저
provenance-aware evidence, time semantics, failure/recovery taxonomy,
deterministic measurement authority를 만든다.

IN SCOPE =
- Request / Quote / Execution / Leg / Destination / Recovery evidence
- Quote Time, Inclusion, Finality, Relay, Swap, Bridge, Completion, Recovery, Compensation 시간
- source chain과 destination chain의 finality criterion
- provider telemetry, chain evidence, independent indexer reconciliation
- missing data, stale data, conflicting source 처리
- failure cause와 provider-controllability
- last-known asset location
- Recovery State와 evidence completeness
- Metric / SLO / Commercial SLA / Compensation / Insurance 구분
- Signed Quote에 포함할 측정가능 조건
- breach, exempt external event, unresolved state
- receipt schema와 dispute evidence
- BM1 attribution, BM3 report, BM4 history용 공통 evidence interface

OUT OF SCOPE =
- AI model architecture와 provider ranking
- 실제 route failover 실행
- commercial bond size·reserve·보험 법률 확정
- institution policy UX/API
- provider eligibility의 사업정책
- 특정 indexer를 유일한 adjudicator로 지정
- 전역 finality·atomicity·원금보장

LOCAL HARD LOCKS =
- Metric ≠ SLO ≠ Commercial SLA ≠ Compensation ≠ Insurance를 유지한다.
- “destination tx observed”와 “agreed finality reached”를 구분한다.
- provider API status 하나를 최종 법적 진실로 사용하지 않는다.
- single indexer를 단독 breach authority로 사용하지 않는다.
- provider self-report는 독립 증거가 없으면 confidence를 낮춘다.
- timestamp source, clock semantics, freshness를 명시한다.
- missing evidence를 성공으로 간주하지 않는다.
- chain halt, bridge halt, user error, provider-controlled failure를 분리한다.
- global atomic revert 또는 guaranteed delivery를 암시하지 않는다.
- raw PII와 기관 민감정보를 public evidence에 포함하지 않는다.

PRESERVED RECOVERY STATES =
COMPLETED
REFUNDED_TO_SOURCE
RECOVERED_AT_SWAP_CHAIN
RECOVERED_AT_INTERMEDIATE
COMPENSATION_PENDING
MANUAL_RECOVERY_REQUIRED
EXEMPT_EXTERNAL_EVENT
UNRESOLVED

MINIMUM TIME MODEL =
Quote Time
Quote Expiry
Authorization Time
Source Inclusion Time
Source Finality Time
Leg Start / End Time
Relay Time
Swap Time
Bridge Time
Destination Inclusion Time
Destination Finality Time
Total Completion Time
Failure Detection Time
Recovery Start / End Time
Compensation Decision / Payout Time

EVIDENCE HIERARCHY =
1. source transaction / state and cryptographic protocol evidence
2. destination transaction / state
3. packet acknowledgement, timeout, bridge-specific state
4. independent indexer reconciliation
5. provider-signed telemetry
6. operator narrative or manual incident note

RULE =
낮은 계층의 증거만 존재하면 그 사실을 표시하고 confidence를 과장하지 않는다.

DEPENDENCIES =
INPUT FROM CH-01 =
campaign attribution event와 revenue evidence 요구

INPUT FROM CH-03 =
모델 학습에 필요한 feature/label 요구와 leakage 방지 조건

INPUT FROM CH-04 =
route leg, failover point, split/aggregate completion, recovery invariant

INPUT FROM CH-05 =
institutional report와 service class가 요구하는 SLO

INPUT FROM CH-06 =
provider capability/history와 evidence freshness reference

INPUT FROM CH-07 =
breach, exempt event, compensation, legal responsibility boundary

OUTPUT TO ALL =
canonical telemetry, time, failure, recovery, SLO, evidence semantics

REQUIRED OUTPUTS =
BM2-EVID-01 = TELEMETRY_AND_PROVENANCE_SCHEMA
BM2-EVID-02 = TIME_AND_FINALITY_SEMANTICS
BM2-EVID-03 = FAILURE_RECOVERY_CONTROLLABILITY_TAXONOMY
BM2-EVID-04 = INTERCHAIN_SLO_DICTIONARY
BM2-EVID-05 = SLA_BREACH_EXCEPTION_EVIDENCE_RULE
BM2-EVID-06 = INDEPENDENT_RECONCILIATION_AND_DISPUTE_PROTOCOL

DECISION QUESTIONS =
- 어떤 event가 completion을 증명하는가?
- finality는 chain별로 어떤 profile로 정의되는가?
- provider-controllable breach와 external event를 어떻게 구분하는가?
- 자산의 last-known location을 언제 확정할 수 있는가?
- 어떤 missingness가 SLA 판정을 HOLD로 만드는가?
- on-chain minimum receipt와 off-chain detailed evidence의 경계는 무엇인가?
- 어떤 metric만 M3 bounded pilot에서 계약가능한가?

PASS =
- pilot-scope route의 completion/recovery를 재현할 수 있다.
- timestamp·finality·provenance가 명시된다.
- provider self-report와 independent evidence를 조정할 규칙이 있다.
- SLO와 breach가 객관적으로 판정된다.
- last-known asset location이 failure simulation에서 복원된다.

HOLD =
- failure/recovery label이 부족하다.
- source disagreement를 해소할 규칙이 없다.
- finality criterion 또는 time semantics가 불명확하다.
- evidence visibility가 privacy boundary와 충돌한다.

KILL / SCOPE REDUCTION =
- 선택 서비스가 객관적으로 측정되지 않는다.
- recovery state를 재구성할 수 없다.
- commercial rights가 단일 provider의 임의 status에 의존한다.
- SLA exposure가 evidence quality보다 앞선다.

CURRENT START POINT =
AI와 SLA 가격보다 먼저 BM2-EVID-01~03을 고정한다.


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
