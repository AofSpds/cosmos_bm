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
