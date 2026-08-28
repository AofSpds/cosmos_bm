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
12. VALIDATION / HANDOFF / REPORTING
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
