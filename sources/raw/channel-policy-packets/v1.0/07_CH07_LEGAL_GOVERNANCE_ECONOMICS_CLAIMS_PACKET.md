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
