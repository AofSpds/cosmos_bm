# COSMOS HUB BM v1.2 — CHANNEL POLICY PACKETS (8)

Date: 2026-08-29 KST



---

<!-- SOURCE FILE: 00_CH00_INTEGRATION_OWNER_DECISIONS_PACKET.md -->

# COSMOS HUB BM v1.2 — INTEGRATION / OWNER DECISIONS

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-00

CHANNEL =
COSMOS HUB BM v1.2 — INTEGRATION / OWNER DECISIONS

PACKET_TYPE =
INTEGRATION CONTROL / OWNER DECISION GOVERNANCE / CROSS-CHANNEL CONFLICT RESOLUTION / NO SPECIALIST REDESIGN

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
OR-01~OR-09 중 실제 선택이 필요하거나 Revision Scope Candidate가 닫힐 때


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
CH00-INT-D

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
전체 채널의 Control Tower / Authority Registry / Decision Integration Desk

PRIMARY QUESTION =
각 전문 채널의 Candidate를 네 개 BM과 Thin Core / Rich Edges 안에서
어떻게 통합하고, 무엇을 Owner 결정으로 승격하며,
v1.2 본문·기술부록·별도 연구문서 중 어디에 반영할 것인가?

MISSION =
- 공통 기준선, 권한, 상태, 용어를 유지한다.
- 채널 간 객체·정의·의존성 충돌을 해결한다.
- Owner Decision Queue를 관리한다.
- 전문 채널 Handoff를 ACCEPT / RETURN / HOLD / REJECT한다.
- M0–M6, T0–T9, G0–G8의 통합 상태를 추적한다.
- Revision Scope Candidate를 작성한다.
- 결정의 supersession과 historical record를 보존한다.

IN SCOPE =
- Channel Scope Registry와 Authority Map
- Canonical Object / Term Registry
- Cross-channel Dependency Map
- Decision Register와 Supersession Log
- OR-01~OR-09 Owner Decision Sheet
- Shared Gate 상태와 독립 Hold/Kill 경계
- Main Text / Technical Annex / Companion Research Paper 배치
- v1.2 Revision Scope Candidate
- 문서별 Claim Ceiling
- 각 결정이 어느 BM·Track·문단에 반영되는지 추적

OUT OF SCOPE =
- AI 모델 세부 설계
- SLA metric 산식 세부 결정
- Multi-path 상태머신 저작
- Enterprise API 필드 저작
- Registry 필드의 도메인별 세부 판단
- 법률 자문·계약 체결·회계 처리 확정
- 실제 배포·파일럿·거래 실행
- 전문 채널의 미해결 문제를 통합 결론으로 덮는 행위

LOCAL HARD LOCKS =
- 전문 채널의 의미를 유지한 채 통합하며 임의 재작성하지 않는다.
- OR-01~OR-09는 Owner의 명시적 결정 없이 자동 승인으로 간주하지 않는다.
- 새로운 공통 객체·공통 계층·제5 BM·Hub 권한 확대는 Owner Decision Required다.
- WATCH 항목을 통합 단계에서 SELECT로 자동 승격하지 않는다.
- 기존 구현을 신규 제안으로, 제안 객체를 현행 구현으로 오표기하지 않는다.
- 통합 편의를 이유로 독립 Kill 경계를 제거하지 않는다.
- 일반적인 동의 표현만으로 생산·실거래·보상·전체 개정 승인을 추정하지 않는다.

CANONICAL SHARED OBJECT OWNERSHIP =
| Shared Object | Primary Owner Channel | CH-00 Role |
|---|---|---|
| Distribution Campaign / Attribution / Revenue Event | CH-01 | BM1 및 Revenue Vault 연결 통합 |
| Telemetry / Metric / SLO / SLA / Recovery Evidence | CH-02 | 공통 의미와 증거권한 통합 |
| AI Prediction / Model Version / Shadow Result | CH-03 | 권한 경계와 성숙도 통합 |
| Route Plan / Leg / Failover / Split / Recovery Invariant | CH-04 | 객체 중복과 실행경계 통합 |
| Structured Intent / Service Class / Policy Profile | CH-05 | BM2·BM4 인터페이스 통합 |
| Asset / Provider / Capability / Incident Record | CH-06 | factual registry와 service catalog 통합 |
| Responsibility / Exposure / Governance / Claim | CH-07 | 전 채널 Gate와 문구 통합 |

OWNER DECISION QUEUE =
OR-01 = B. SELECTIVE FIT 수용 여부
OR-02 = SELECT 3개 핵심 개념 승인 여부
OR-03 = SELECT-LIMITED 개념의 단계별 Gate 적용 승인 여부
OR-04 = Route Diversity / Split Routing을 Existing / Assess로 고정할지
OR-05 = Replay / Agentic / Hedged를 WATCH로 유지할지
OR-06 = Zero-touch / Literal Slicing / RAN-PHY / Hub proprietary router를 REJECT할지
OR-07 = M0–M6 × T0–T9 roadmap Candidate 수용 여부
OR-08 = Option B — Main Text + Technical Annex 잠정 우선 여부
OR-09 = Pre-PoC Claim Ceiling C2 유지 여부

DEFAULT STATUS =
UNDECIDED / DO NOT AUTO-INFER

REQUIRED OUTPUTS =
CH00-01 = CHANNEL_REGISTRY_AND_AUTHORITY_MAP
CH00-02 = CANONICAL_OBJECT_AND_TERM_REGISTRY
CH00-03 = CROSS_CHANNEL_DEPENDENCY_AND_CONFLICT_LOG
CH00-04 = OWNER_DECISION_REGISTER
CH00-05 = INTEGRATED_GATE_STATUS
CH00-06 = V1.2_REVISION_SCOPE_CANDIDATE

INTEGRATION PROCEDURE =
1. 전문 채널이 CHANNEL-SEALED Handoff를 제출한다.
2. CH-00은 범위·Hard Lock·의존성·Claim Ceiling·Owner 필요 여부만 확인한다.
3. 결과는 다음 중 하나다.
   - ACCEPT FOR INTEGRATION
   - RETURN FOR CLARIFICATION
   - HOLD FOR DEPENDENCY
   - REJECT FOR HARD-LOCK CONFLICT
4. ACCEPT라도 Owner 승인이 필요한 항목은 OWNER DECISION REQUIRED로 유지한다.
5. Owner 결정 뒤에만 INTEGRATED 상태로 승격한다.

PASS =
- 네 개 BM 중 명확한 소유 위치가 있다.
- 공통 객체와 의미 충돌이 없다.
- Thin Core / Rich Edges와 독립 Kill 경계를 유지한다.
- 기술·법률·경제·claim 상태가 일치한다.
- 현행 구현과 신규 제안이 구분된다.

HOLD =
- 두 채널이 같은 객체를 다른 의미로 정의한다.
- 선행 데이터·법률·경제성 Gate가 열려 있다.
- Owner 선택 없이는 통합할 수 없는 대안이 남아 있다.

KILL / REJECT =
- 제5 BM 또는 독점 Hub 사업으로 팽창한다.
- AI·Hub 권한을 Hard Lock 이상으로 확대한다.
- C2 초과 claim을 PoC 없이 요구한다.
- 생산·실거래·보상 승인을 묵시적으로 포함한다.

CURRENT START POINT =
STEP 3–5 자료를 기준선으로 등록한다.
각 전문 채널에서 첫 Candidate가 올라오기 전에는 본문 개정을 시작하지 않는다.


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


---

<!-- SOURCE FILE: 01_CH01_BM1_DISTRIBUTION_REVENUE_PACKET.md -->

# COSMOS HUB BM1 — DISTRIBUTION MARKET / REVENUE EVIDENCE

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-01

CHANNEL =
COSMOS HUB BM1 — DISTRIBUTION MARKET / REVENUE EVIDENCE

PACKET_TYPE =
BM1 PRODUCT DESIGN / ATTRIBUTION / ANTI-GAMING / REVENUE EVIDENCE / NO AI DEPENDENCY

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
BM1-DIST-02~06 Candidate가 닫혀 MVP 선택과 경제성 판단이 필요할 때


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
BM1-DIST-D

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
BM1 Product / Market / Revenue Evidence Design Channel

PRIMARY QUESTION =
발행사가 실제로 돈을 내고 반복 사용할
Interchain Asset Distribution Market은 어떤 상품이어야 하며,
성과와 외부매출을 어떻게 조작 저항적으로 증명할 것인가?

MISSION =
BM1을 AI Routing의 선행결과에 종속시키지 않고,
Campaign 계약, attribution, anti-gaming, provider payout,
Revenue Event와 반복 외부매출 증거를 먼저 닫는다.

IN SCOPE =
- Issuer Campaign 등록과 예산·기간·대상 정의
- Provider·Wallet·DEX·Bridge·Analytics actor 역할
- Campaign baseline과 incremental performance
- time-weighted balance, verified holder, liquidity depth, retention
- 30/60/90일 성과창
- wash transfer, self-dealing, circular flow, sybil 방지
- attribution source와 독립 계산
- provider payout, holdback, clawback, dispute
- Revenue Event와 Revenue Vault 연결
- contracted / accrued / received revenue 구분
- ATOM purchase / Community Pool deposit의 별도 증거
- willingness-to-pay, renewal, unit economics
- 3~6개월 Distribution MVP 범위와 Kill 조건

OUT OF SCOPE =
- AI route model 설계
- live failover·split·hedged execution
- BM2 SLA의 metric·breach 확정
- BM3 institution policy/API 설계
- BM4 공통 registry schema 확정
- 법률 당사자·세무·회계의 최종 결론
- Hub 자체 마케팅 대행사 또는 독점 distribution operator 설계

LOCAL HARD LOCKS =
- BM1 시작조건에 AI Routing 성공을 넣지 않는다.
- 거래량·TVL 증가만으로 성과를 인정하지 않는다.
- 내부 토큰 순환이나 보조금 재순환을 외부매출로 기록하지 않는다.
- 발행사·provider self-report만으로 payout을 확정하지 않는다.
- campaign 성과와 일반 시장상승을 분리할 baseline을 정의한다.
- anti-gaming rule은 payout 전에 적용하고 사후 clawback 경로를 둔다.
- Revenue Event는 CONTRACTED / ACCRUED / RECEIVED를 분리한다.
- ATOM 매입과 Community Pool 귀속은 실제 transaction evidence가 있을 때만 실현으로 표기한다.
- BM1 데이터 수집은 BM2/AI 연구에 재사용할 수 있으나 BM1 고객가치를 희석하지 않는다.

CANONICAL OBJECTS =
Distribution Campaign
Issuer
Campaign Budget
Target Asset / Chain / Market
Eligible Provider
Attribution Event
Performance Window
Baseline
Incremental Outcome
Anti-gaming Flag
Payout Record
Holdback / Clawback
Revenue Event
Revenue Vault Reference
Campaign Receipt

MINIMUM PERFORMANCE FRAME =
1. Baseline:
   캠페인 전 상태와 자연증가 추세
2. Increment:
   캠페인으로 귀속 가능한 추가 성과
3. Quality:
   실제 holder, depth, retention, 사용성
4. Integrity:
   wash·self-dealing·순환흐름 제외
5. Economics:
   issuer payment - provider payout - operating cost = protocol contribution
6. Persistence:
   renewal과 30/60/90일 유지

DEPENDENCIES =
INPUT FROM CH-02 =
검증 가능한 event, timestamp, provenance, receipt semantics

INPUT FROM CH-06 =
provider capability와 factual history

INPUT FROM CH-07 =
계약당사자, payout·clawback, revenue recognition, competition boundary

OUTPUT TO CH-02 =
campaign attribution에 필요한 telemetry와 evidence 요구사항

OUTPUT TO CH-06 =
campaign provider capability와 performance-history 후보

OUTPUT TO CH-00 =
BM1 MVP, revenue definition, 상업 roadmap에 영향을 주는 Decision Handoff

REQUIRED OUTPUTS =
BM1-DIST-01 = CURRENT_MARKET_AND_ACTOR_BASELINE
BM1-DIST-02 = DISTRIBUTION_CAMPAIGN_OBJECT_AND_FLOW
BM1-DIST-03 = ATTRIBUTION_AND_ANTI_GAMING_SPEC
BM1-DIST-04 = PROVIDER_PAYOUT_HOLDBACK_CLAWBACK_RULE
BM1-DIST-05 = REVENUE_EVENT_AND_VAULT_EVIDENCE_MODEL
BM1-DIST-06 = DISTRIBUTION_MVP_AND_WTP_GATE

DECISION QUESTIONS =
- 어떤 성과를 issuer가 유료로 구매하는가?
- 성과의 incremental attribution은 무엇으로 증명하는가?
- Provider 지급은 언제 확정되는가?
- 어떤 gaming signal이 지급보류·clawback을 발생시키는가?
- Hub/CosmWasm에 남길 최소 state와 off-chain 계산은 무엇인가?
- 실제 외부매출이 Revenue Vault까지 어떻게 추적되는가?
- 3~6개월 MVP에서 반드시 검증할 한 가지 고객가치는 무엇인가?

PASS =
- issuer가 이해하고 지불할 outcome이 명확하다.
- attribution과 anti-gaming을 독립적으로 재현할 수 있다.
- payout과 revenue state가 구분된다.
- 외부 paid revenue와 renewal evidence가 있다.
- AI 없이도 BM1 MVP가 성립한다.

HOLD =
- 성과 baseline이 불안정하거나 third-party calculation이 불가능하다.
- payout이 provider self-report에 과도하게 의존한다.
- 고객이 관심은 있으나 가격·계약·renewal 증거가 없다.

KILL / PIVOT =
- 유료 수요가 반복적으로 확인되지 않는다.
- gaming 제거 후 실질 성과가 남지 않는다.
- 운영·측정·provider 비용이 gross revenue를 지속적으로 초과한다.
- BM1이 단순 보조금 배분 또는 내부 토큰 순환으로 축소된다.

CURRENT START POINT =
AI·6G를 앞세우지 말고 Campaign Product와 Revenue Evidence를 먼저 정의한다.


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


---

<!-- SOURCE FILE: 02_CH02_BM2_OBSERVABILITY_SLO_SLA_PACKET.md -->

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


---

<!-- SOURCE FILE: 03_CH03_BM2_AI_SKIP_GO_ROUTING_PACKET.md -->

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


---

<!-- SOURCE FILE: 04_CH04_BM2_MULTIPATH_FAILOVER_RECOVERY_PACKET.md -->

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


---

<!-- SOURCE FILE: 05_CH05_BM3_ENTERPRISE_GATEWAY_INTENT_PACKET.md -->

# COSMOS HUB BM3 — ENTERPRISE GATEWAY / STRUCTURED INTENT

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-05

CHANNEL =
COSMOS HUB BM3 — ENTERPRISE GATEWAY / STRUCTURED INTENT

PACKET_TYPE =
ENTERPRISE PRODUCT / STRUCTURED INTENT / CAPABILITY EXPOSURE / EXPLICIT AUTHORIZATION / NO DIRECT LLM EXECUTION

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
BM3-ENT-02~06 Candidate가 닫혀 pilot·service class·본문 반영 선택이 필요할 때


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
BM3-ENT-D

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
BM3 Enterprise Product / Structured Intent / Capability Exposure Channel

PRIMARY QUESTION =
기관이 chain·bridge·DEX·router를 직접 조합하지 않고도
정책에 맞는 Interchain 서비스를 사용할 수 있게 하려면,
어떤 structured abstraction과 운영상품이 필요한가?

MISSION =
One-Connection Gateway의 고객가치를
Structured Intent, Capability Catalog, Policy Adapter,
Institutional Receipt와 Reconciliation으로 구체화한다.
자연어는 선택적 초안 인터페이스일 뿐 authoritative하지 않다.

IN SCOPE =
- enterprise customer problem과 integration cost
- Service Intent schema
- Service Class
- Policy Profile
- Route Constraint
- SLA Template reference
- Receipt Profile
- Recovery Policy
- Capability Catalog interface
- deterministic syntax/semantic validation
- policy conflict detection
- fee, route, finality, recovery disclosure
- institution authorization
- gateway API, endpoint, monitoring, alert
- institutional receipt와 reconciliation
- incident / upgrade coordination
- public/basic layer와 paid enterprise layer
- pilot partner, WTP, support economics
- optional natural-language draft assistant

OUT OF SCOPE =
- LLM 직접 transaction 실행
- AI의 institution policy 변경
- raw KYC/PII on-chain 저장
- Hub 단일 독점 enterprise operator
- route model·failover engine 자체 구현
- commercial SLA 법률 확정
- “automated regulatory compliance” claim

LOCAL HARD LOCKS =
- Natural Language → Structured Intent → Validation → Disclosure → Confirmation 순서를 유지한다.
- 자연어 해석 결과는 초안이며 structured fields가 authoritative하다.
- unsupported, ambiguous, conflicting intent는 fail closed한다.
- 실제 route·fee·finality·recovery 위험을 추상화 뒤에 숨기지 않는다.
- institution authorization과 credential boundary를 유지한다.
- Gateway는 경쟁 가능한 operator product이며 Hub 독점 고객창구가 아니다.
- institution policy 원문과 PII는 off-chain/access-controlled로 둔다.
- capability와 SLA는 CH-02·CH-06의 factual record를 참조한다.
- “one connection”을 one provider monopoly로 해석하지 않는다.
- paid enterprise value는 API 호출 자체가 아니라 integration·monitoring·reconciliation·incident 절감으로 증명한다.

INITIAL SERVICE CLASSES =
STANDARD
LOW-COST
FAST
RISK-ADJUSTED
ASSURED
INSTITUTIONAL

SAFE PROCESSING FLOW =
Optional Natural-language Draft
→ Structured Intent
→ Syntax / Semantic Validation
→ Policy Conflict Detection
→ Candidate Capability / Route / SLA Plans
→ Fee / Route / Finality / Recovery Disclosure
→ Institution Confirmation
→ Deterministic Transaction Construction
→ Cryptographic Verification
→ Execution
→ Institutional Receipt / Reconciliation

MINIMUM STRUCTURED INTENT FIELDS =
ASSET
AMOUNT
SOURCE
DESTINATION
MAX_TOTAL_COST
MINIMUM_RECEIVE
TARGET_COMPLETION
FINALITY_PROFILE
RELIABILITY_CLASS
ALLOWED_PROVIDER_POLICY
ALLOWED_PROTOCOL_POLICY
MAX_EXPOSURE
RECOVERY_POLICY
RECEIPT_PROFILE
AUTHORIZATION_REFERENCE

DEPENDENCIES =
INPUT FROM CH-02 =
SLO, finality, receipt, evidence completeness, recovery semantics

INPUT FROM CH-04 =
route/failover/split capability와 user disclosure 요구

INPUT FROM CH-06 =
provider/asset/capability factual catalog

INPUT FROM CH-07 =
custody, agency, data, contract, support, jurisdiction boundary

OUTPUT TO CH-01 =
issuer campaign enterprise distribution interface가 필요한 경우 요구사항

OUTPUT TO CH-00 =
service classes, common intent objects, enterprise roadmap와 문서 반영 결정

REQUIRED OUTPUTS =
BM3-ENT-01 = ENTERPRISE_CUSTOMER_PROBLEM_AND_ACTOR_MAP
BM3-ENT-02 = STRUCTURED_SERVICE_INTENT_SCHEMA
BM3-ENT-03 = SERVICE_CLASS_AND_CAPABILITY_MAPPING
BM3-ENT-04 = DETERMINISTIC_VALIDATION_DISCLOSURE_AUTHORIZATION_FLOW
BM3-ENT-05 = ENTERPRISE_API_RECEIPT_RECONCILIATION_MODEL
BM3-ENT-06 = PILOT_WTP_SUPPORT_ECONOMICS_GATE

DECISION QUESTIONS =
- 기관이 실제로 줄이고 싶은 integration work는 무엇인가?
- 어떤 intent field가 필수이며 어떤 것은 선택인가?
- service class는 측정 가능한 capability와 어떻게 연결되는가?
- conflicting intent와 unsupported route를 어떻게 fail closed하는가?
- 기관이 승인 전에 반드시 봐야 할 fee/risk/finality/recovery 정보는 무엇인가?
- public Hub layer와 paid operator layer의 경계는 무엇인가?
- protocol revenue가 enterprise operator revenue에서 어떻게 추적되는가?

PASS =
- structured intent가 명확하고 invalid/conflicting request를 막는다.
- 기관이 material risk를 보고 명시적으로 승인한다.
- capability/SLA mapping이 factual evidence에 연결된다.
- integration time/cost 또는 reconciliation/support 부담 절감이 측정된다.
- paid 또는 계약상 credible demand가 있다.
- 복수 operator 경쟁과 switching이 가능하다.

HOLD =
- 고객 관심은 있으나 책임·데이터·support economics가 불명확하다.
- intent abstraction이 지나치게 복잡하거나 correction rate가 높다.
- capability catalog가 factual evidence보다 marketing label에 의존한다.

KILL / PIVOT =
- abstraction이 material route/finality/recovery risk를 숨긴다.
- Gateway가 사실상 custody나 discretionary execution을 떠안는다.
- paid demand가 없고 protocol share를 투명하게 귀속할 수 없다.
- LLM direct execution 없이는 제품이 성립하지 않는다.

CURRENT START POINT =
BM3-ENT-01과 BM3-ENT-02를 먼저 닫고 UI나 LLM 구현은 후행한다.


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


---

<!-- SOURCE FILE: 06_CH06_BM4_REGISTRY_PROVIDER_MARKET_PACKET.md -->

# COSMOS HUB BM4 — ASSET & SERVICE REGISTRY / PROVIDER MARKET

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-06

CHANNEL =
COSMOS HUB BM4 — ASSET & SERVICE REGISTRY / PROVIDER MARKET

PACKET_TYPE =
FACTUAL REGISTRY / OPEN PROVIDER MARKET / NEUTRALITY / CONFLICT ARBITRATION / NO APPROVAL BADGE

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
BM4-REG-01~06 Candidate가 닫혀 공통 객체·neutrality·registry 범위 선택이 필요할 때


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
BM4-REG-D

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
BM4 Factual Registry / Open Provider Market / Neutrality Channel

PRIMARY QUESTION =
어떤 Asset와 Provider가 무엇을 지원하고,
어떤 서명·증거·성과·사고 이력을 가졌는지를
중립적이고 검증 가능하게 어떻게 기록할 것인가?

MISSION =
Registry를 승인·보증 badge가 아니라 factual evidence interface로 설계한다.
Provider eligibility, model ranking, open entry, switching,
concentration과 conflict arbitration을 분리한다.

IN SCOPE =
- Asset Record
- issuer-declared canonical representation과 signature
- reserve/document/attestation pointer와 issuer 표시
- Service Provider Record
- Capability Record와 supported routes/protocols
- signed quote reference
- evidence freshness와 revocation
- historical latency/failure/recovery reference
- incident history
- SLA tier와 bond reference
- model/version reference의 제한적 audit use
- deterministic eligibility
- provider ranking과 confidence
- open entry, switching, newcomer evaluation
- concentration KPI
- self-reported telemetry discount/corroboration
- conflicting capability/representation/quote detection
- deterministic arbitration과 audit trail
- public/on-chain minimum과 off-chain detail 경계

OUT OF SCOPE =
- Hub Approved / Safe Asset / Guaranteed Provider / Regulatory Compliant badge
- raw KYC/PII, trade secret, proprietary model feature 공개
- provider의 route engine 운영
- AI가 eligibility를 단독 결정
- 특정 provider를 default monopoly로 지정
- 법률적 인증·인가를 Registry가 대체하는 구조

LOCAL HARD LOCKS =
- Registry는 사실·서명·출처·시점·이력만 기록한다.
- issuer-declared와 independently verified를 구분한다.
- provider self-report와 independent evidence를 구분한다.
- factual capability와 performance score를 분리한다.
- deterministic eligibility와 model ranking을 분리한다.
- score가 낮다고 자동 퇴출하거나 높다고 승인 badge를 주지 않는다.
- confidence interval, freshness, missing data를 표시한다.
- 신규 provider가 데이터 부족으로 영구 배제되지 않도록 evaluation path를 둔다.
- top-provider concentration과 switching friction을 측정한다.
- incident history는 범위·근거·해결상태와 함께 기록한다.
- 상세 telemetry·민감정보는 off-chain에 두고 on-chain에는 최소 reference만 둔다.
- Hub가 provider와 직접 경쟁하거나 proprietary data advantage를 만들지 않는다.

FACTUAL LABELS ALLOWED =
Supported Route
Signed Capability
Evidence Source
Evidence Freshness
Measured Historical Result
Attestation Issuer
Incident Record
Bond Reference
Revocation Status
Confidence / Missingness

LABELS PROHIBITED =
Hub Approved
Safe Asset
Guaranteed Provider
Regulatory Compliant
Best Provider
Risk Free
Fully Verified

MINIMUM PROVIDER RECORD =
provider_id
operator_identity_reference
service_types
supported_assets
supported_routes
supported_protocols
jurisdiction_or_policy_reference_if_disclosed
capability_signature
quote_interface
evidence_sources
telemetry_freshness
historical_result_reference
incident_reference
bond_reference
revocation_status
last_updated
schema_version

NEUTRALITY CONTROLS =
Open capability and quote schema
Multiple providers where market permits
Switching path
Deterministic eligibility
Ranking/eligibility separation
Confidence and data-quality disclosure
Top-provider share and concentration trend
Newcomer evaluation quota/path
Self-report corroboration
Public conflict/arbitration rule
No exclusive mandatory operator

DEPENDENCIES =
INPUT FROM CH-01 =
distribution provider roles와 campaign performance evidence

INPUT FROM CH-02 =
canonical evidence, freshness, incident, SLO/history semantics

INPUT FROM CH-03 =
model output의 confidence/version; eligibility와 분리할 조건

INPUT FROM CH-04 =
route/failover/split capability와 recovery evidence

INPUT FROM CH-05 =
capability catalog와 structured intent mapping 요구

INPUT FROM CH-07 =
competition, discrimination, attestation, liability, privacy boundary

OUTPUT TO CH-00 =
공통 Asset/Provider/Capability 객체와 neutrality decisions

REQUIRED OUTPUTS =
BM4-REG-01 = ASSET_RECORD_AND_ISSUER_DECLARATION_SCHEMA
BM4-REG-02 = PROVIDER_AND_CAPABILITY_RECORD_SCHEMA
BM4-REG-03 = EVIDENCE_FRESHNESS_INCIDENT_REVOCATION_MODEL
BM4-REG-04 = ELIGIBILITY_RANKING_AND_CONFIDENCE_SEPARATION
BM4-REG-05 = OPEN_ENTRY_SWITCHING_CONCENTRATION_POLICY
BM4-REG-06 = CONFLICT_DETECTION_AND_DETERMINISTIC_ARBITRATION

DECISION QUESTIONS =
- public chain에 남길 최소 factual record는 무엇인가?
- issuer declaration과 external attestation을 어떻게 구분하는가?
- provider capability와 measured history를 어떻게 연결하는가?
- stale/conflicting evidence를 어떻게 표시하고 revoke하는가?
- eligibility와 score를 어떤 규칙으로 분리하는가?
- 신규 provider와 지배적 provider 간 feedback loop를 어떻게 통제하는가?
- BM3 capability catalog는 Registry의 어떤 field를 참조하는가?

PASS =
- record가 서명·source·freshness·version에 바인딩된다.
- factual claim과 opinion/ranking이 구분된다.
- provider switching과 open entry가 가능하다.
- concentration과 self-report dependence가 측정된다.
- conflict resolution이 deterministic하고 auditable하다.
- misleading approval/compliance label이 없다.

HOLD =
- market이 너무 얇아 비교 가능한 provider가 없다.
- 핵심 데이터가 self-reported only다.
- privacy/trade-secret boundary가 불명확하다.
- score가 factual history보다 모델 추정에 과도하게 의존한다.

KILL / PIVOT =
- Registry가 사실상 승인·보증 기관으로 오인된다.
- 특정 provider가 mandatory exclusive operator가 된다.
- ranking이 opaque monopoly feedback을 만들고 switching이 불가능하다.
- record를 유지하기 위해 raw PII·trade secret 공개가 필요하다.

CURRENT START POINT =
BM4-REG-01~03 factual schema를 먼저 닫고,
score·ranking·market design은 그 뒤에 논의한다.


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


---

<!-- SOURCE FILE: 07_CH07_LEGAL_GOVERNANCE_ECONOMICS_CLAIMS_PACKET.md -->

# COSMOS HUB v1.2 — LEGAL / GOVERNANCE / ECONOMICS / CLAIMS

[CHANNEL GOVERNANCE / SCOPE / EXECUTION PACKET]

PROJECT =
COSMOS HUB BM IMPROVEMENT

TARGET =
COSMOS HUB BM v1.2 CONCEPT INTEGRATION ROADMAP CANDIDATE

CHANNEL_ID =
CH-07

CHANNEL =
COSMOS HUB v1.2 — LEGAL / GOVERNANCE / ECONOMICS / CLAIMS

PACKET_TYPE =
CROSS-CUTTING GATE / RESPONSIBILITY / GOVERNANCE / ECONOMICS / CLAIM MANAGEMENT / NO PRODUCT REDESIGN

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
LGEC-01~06에서 Owner 선택·external counsel·pilot gate가 필요한 항목이 정리될 때


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
LGEC-D

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
Cross-cutting Legal / Governance / Economics / Claim Gate Channel

PRIMARY QUESTION =
기술적으로 가능한 Candidate가
법적 책임, 거버넌스 권한, 경제성, 중립성, 표현 강도 측면에서
실행 가능한 상품이 될 수 있는가?

MISSION =
다른 채널의 제품을 대신 설계하지 않는다.
각 Candidate에 책임·권한·노출·수익·claim의 Go/Hold/Kill 조건을 부여하고,
Owner와 CH-00이 통합 결정을 내릴 수 있는 boundary memo를 만든다.

IN SCOPE =
- Router, Provider, Gateway, Wallet, Hub, Evidence Operator의 책임분리
- contract party와 invoice/revenue flow
- custody, agency, discretionary execution 경계
- 잘못된 recommendation과 policy translation 책임
- provider-controllable breach와 external event
- Provider Bond, reserve, exposure cap, compensation ceiling
- SLA와 guarantee/insurance의 경계
- partial completion, duplicate execution, recovery liability
- data privacy, PII, institution policy, trade secret
- AI model responsibility, explainability, discrimination, concentration
- open provider competition과 proprietary data lock-in
- governance authority: admin key, pause, upgrade, revocation, dispute
- willingness-to-pay, unit economics, support/incident cost
- contracted / accrued / received revenue
- ATOM purchase / Community Pool evidence
- Claim Ladder C0–C5와 문서·채널별 허용문구
- adversarial review와 residual risk
- 필요 시 external counsel / audit가 필요한 질문 목록

OUT OF SCOPE =
- BM1 campaign product를 대신 설계
- BM2 telemetry·model·state machine을 대신 작성
- BM3 API UX를 대신 작성
- BM4 factual field를 대신 정함
- 법률의견서·규제승인·보험인가가 이미 완료됐다고 주장
- production contract 체결
- 투자·수익을 보장하는 문구 작성

LOCAL HARD LOCKS =
- 법률 검토 전 compensation을 보험·보증으로 표현하지 않는다.
- 기술적으로 controllable하지 않은 사건에 무제한 책임을 부과하지 않는다.
- exposure, reserve, bond, payout ceiling이 없으면 commercial pilot을 PASS하지 않는다.
- “non-custodial” 표방만으로 custody/agency risk가 사라진다고 가정하지 않는다.
- model recommendation과 final authorization의 책임을 분리한다.
- provider rank가 discrimination 또는 market concentration을 강화하는지 검토한다.
- raw PII/KYC와 institution policy를 public chain에 두지 않는다.
- Revenue는 계약발표가 아니라 실제 received external inflow를 중심으로 구분한다.
- 6G·AI·SLA 표현은 source status와 measured maturity를 넘지 않는다.
- formal legal conclusion이 필요한 항목은 COUNSEL REQUIRED로 표시한다.
- 이 채널은 제품을 무기한 블로킹하지 않고 정확한 HOLD 조건과 최소 closure evidence를 제시한다.

CLAIM LADDER =
C0 — 내부 가설
C1 — 구조적 유사성·정렬
C2 — 공식 연구를 참조한 선택적 설계
C3 — bounded PoC에서 실제 적용·측정
C4 — exact scope가 공개된 operating pilot
C5 — 실제 적합성평가·인증 후

PRE-POC ALLOWED EXAMPLES =
6G-era network-orchestration research-informed
Selected autonomous-network management principles adapted to Interchain
Architecturally aligned with intent-driven management and service-assurance research
Bounded AI-assisted Interchain orchestration roadmap

PROHIBITED =
6G Blockchain
6G-compliant Cosmos Hub
6G-certified Interchain
First 6G Chain
IMT-2030 compliant
3GPP 6G implemented
Guaranteed Delivery
Risk-free Provider
Insurance-backed — 실제 인가·계약 근거 없을 때
Global Atomic Revert
Principal Protection

RESPONSIBILITY QUESTIONS =
- 누가 quote를 발행하고 누가 execution plan을 만든다?
- 누가 route policy를 승인하고 transaction을 서명한다?
- 누가 evidence를 수집하고 breach를 판정한다?
- 누가 recovery를 수행하고 비용을 부담한다?
- 누가 compensation을 지급하며 최대 exposure는 얼마인가?
- Hub/CosmWasm는 규칙·reference만 제공하는가, 계약 당사자인가?
- enterprise operator revenue에서 protocol share는 어떻게 귀속되는가?
- pause, upgrade, key, revocation, dispute authority는 누구에게 있는가?

DEPENDENCIES =
INPUT FROM CH-01 =
campaign 계약, payout, clawback, revenue flow, WTP

INPUT FROM CH-02 =
measurable breach, exception, evidence authority

INPUT FROM CH-03 =
model role, calibration, discrimination, concentration, operating cost

INPUT FROM CH-04 =
duplicate, partial leg, recovery, capital lock, accounting risk

INPUT FROM CH-05 =
institution authorization, data, custody/agency, support responsibility

INPUT FROM CH-06 =
attestation, factual label, provider neutrality, revocation

OUTPUT TO ALL =
GO / HOLD / KILL boundary, residual risk, claim ceiling, Owner issues

OUTPUT TO CH-00 =
integrated legal-governance-economic recommendation과 Revision Scope constraints

REQUIRED OUTPUTS =
LGEC-01 = LEGAL_BOUNDARY_AND_RESPONSIBILITY_MATRIX
LGEC-02 = GOVERNANCE_AUTHORITY_PAUSE_UPGRADE_DISPUTE_MAP
LGEC-03 = ECONOMIC_VIABILITY_RESERVE_EXPOSURE_MODEL
LGEC-04 = CLAIM_LADDER_AND_CHANNEL_CLAIM_REGISTER
LGEC-05 = INTEGRATED_ADVERSARIAL_FINDINGS
LGEC-06 = COUNSEL_AUDIT_AND_OWNER_DECISION_ISSUE_LIST

GO =
- 책임주체와 controllable event가 명확하다.
- amount/exposure/reserve/pause가 bounded하다.
- data와 authority가 least-privilege다.
- WTP와 operating economics가 plausibly positive다.
- provider competition과 switching을 유지한다.
- claim이 evidence maturity와 일치한다.

HOLD =
- 법률 당사자, insurance/custody/agency, privacy classification이 미해결이다.
- WTP는 있으나 support·incident·compensation 비용이 불명확하다.
- governance key, pause, upgrade, dispute 권한이 닫히지 않았다.
- source status와 public wording이 불일치한다.

KILL / REJECT =
- 책임과 exposure가 수익에 비해 unbounded하다.
- product가 사실상 Hub custody·guarantee·exclusive operation을 요구한다.
- provider discrimination/monopoly feedback을 통제할 수 없다.
- 원금보장·보험·규제적합성·6G compliance 과장이 제품가치의 핵심이 된다.
- 정확한 증거 없이 financial rights를 자동 집행해야만 성립한다.

CHANNEL OPERATING RULE =
각 채널의 Candidate를 받은 뒤,
“문제 있음”으로 끝내지 말고 다음 형식으로 반환한다.

OBJECTION =
EVIDENCE =
RESPONSE =
RESIDUAL RISK =
MINIMUM CLOSURE EVIDENCE =
ROADMAP IMPACT =
GO / HOLD / KILL =

CURRENT START POINT =
LGEC-01 책임행렬과 LGEC-04 Claim Register를 먼저 고정한다.


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
