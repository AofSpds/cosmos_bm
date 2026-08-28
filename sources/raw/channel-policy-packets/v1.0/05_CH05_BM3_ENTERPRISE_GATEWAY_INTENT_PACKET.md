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
