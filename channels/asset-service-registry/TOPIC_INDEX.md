# CH-06 Topic Index and Owner Decision Map

```text
PROJECT = COSMOS HUB BM IMPROVEMENT
CHANNEL = CH-06 ASSET & SERVICE REGISTRY
FORMAL_NAME = BM4 Asset & Service Registry / Provider Market
STATUS = CANDIDATE / NAVIGATION AND MEMORY AID
SEMANTIC_AUTHORITY = BM_MASTER
OWNER_DECISION_EFFECT = NONE UNTIL EXPLICIT OWNER DECISION
```

This file is a detailed navigation and continuity aid. It does not replace `CHANNEL.md`, create an Owner decision, seal the channel, or authorize implementation.

## 0. Standing response and tagging rule

Every substantive CH-06 response follows this order:

1. **쉽게 설명** — non-specialist explanation and concrete example.
2. **하드코어 설계** — object model, state machine, evidence, policy, threat, interface, and gate details.
3. **현재 상태** — LOCKED / CANDIDATE / OPEN / HOLD / REJECTED.
4. **오너 질문** — tagged `BM4-OQ-###`.
5. **결정 포인트** — tagged `BM4-DP-###`; a decision point is not an Owner decision.
6. **응답 하단 인덱스** — current topic, completed topics, open questions, pending decisions, dependencies, and next exact action.

Tag grammar:

- `[LOCKED]` — already fixed by Owner/common/channel hard locks.
- `[CANDIDATE]` — channel recommendation only.
- `[OWNER-Q: BM4-OQ-###]` — question requiring an eventual Owner answer.
- `[DECISION-PENDING: BM4-DP-###]` — selectable design decision; not yet decided.
- `[PROJECT-OWNER-Q: OR-##]` — upstream STEP 3–5 Owner-review question.
- `[DEPENDENCY: CH-##]` — requires another channel's input or interface.
- `[UNKNOWN]` — evidence or operating fact is not established.
- `[HOLD]` — do not close until a stated dependency or evidence gate is satisfied.
- `[REJECTED]` — prohibited by hard lock or current concept selection.

Existing Candidate decision records remain:

- `BM4-REG-D-0001` — factual registry only; no approval/safety/compliance badge.
- `BM4-REG-D-0002` — deterministic eligibility is separate from ranking; conflict resolution is public and deterministic.
- `BM4-REG-D-0003` — open competition/switching and off-chain sensitive-data boundary.

They are not Owner decisions.

---

# TOPIC 00 — Registry role, users, and non-role boundary

## 쉽게 설명

Registry는 “좋은 자산·좋은 사업자 인증소”가 아니라 **누가 무엇을 지원한다고 말했고, 어떤 증거가 있으며, 언제 갱신됐고, 어떤 사고와 취소 이력이 있는지를 확인하는 공개 사실 장부**다.

주요 사용자는 자산 발행자, 라우터·릴레이어·브리지·DEX·게이트웨이 사업자, 지갑, 기업 고객, 독립 증거 운영자, 감사자, 거버넌스다.

## 하드코어 범위

- authoritative fact와 assertion을 분리한다.
- issuer declaration, provider self-report, independent observation, cryptographic verification, third-party attestation을 구분한다.
- `REGISTERED ≠ APPROVED ≠ SAFE ≠ COMPLIANT ≠ GUARANTEED`를 스키마와 UX에서 강제한다.
- Registry는 route engine, custody layer, transaction authorizer, compliance certifier가 아니다.
- market neutrality, open specification, switching, no mandatory operator를 기본 불변조건으로 둔다.

## 세부 항목

- 사용자·행위자 모델
- Registry 운영 주체와 거버넌스 권한
- 쓰기·갱신·정정·이의제기 권한
- public query와 authenticated write 경계
- 법적 고지와 claim ceiling
- current implementation과 proposal object의 구분

## 태그

- `[LOCKED] factual evidence only`
- `[LOCKED] no Hub Approved/Safe/Compliant/Guaranteed labels`
- `[OWNER-Q: BM4-OQ-001] Registry 운영 주체는 Hub governance, 독립 operator, 다중 operator federation 중 무엇을 우선 후보로 둘 것인가?`
- `[DECISION-PENDING: BM4-DP-001] Registry operating and governance model`
- `[PROJECT-OWNER-Q: OR-02, OR-03, OR-07, OR-09]`

---

# TOPIC 01 — BM4-REG-01 Asset Record / Issuer Declaration Schema

## 쉽게 설명

같은 이름의 토큰이 여러 체인과 브리지에 존재할 수 있으므로, Registry는 **이 자산이 무엇인지, 누가 발행자라고 주장하는지, 원래 어디서 생성됐는지, 지금 보고 있는 표현이 어떤 경로로 만들어졌는지**를 구분해야 한다.

## 하드코어 범위

Asset Record는 자산 자체의 식별과 표현을 분리한다.

- `asset_id`: Registry 내부의 stable identifier
- `origin_chain_id`, `origin_asset_reference`
- `representation_id`: IBC denom, contract address, bridged representation 등
- `representation_path`: origin → bridge/IBC path → current representation
- `issuer_identity_reference`
- `issuer_declaration`, `issuer_signature`, `signed_at`
- decimals, symbol, display name은 식별의 보조값이지 권위값이 아니다.
- document/reserve/attestation pointer는 “내용이 참”이 아니라 “이 문서가 이 선언과 연결됨”만 기록한다.
- canonical claim, equivalence claim, redemption claim을 서로 다른 assertion type으로 둔다.
- version, supersedes, effective_from, expires_at, revocation_status를 둔다.
- conflicting representation은 삭제하지 않고 conflict set으로 묶는다.

## 세부 항목

1. 자산 고유 ID와 사람이 보는 ticker 분리
2. origin asset과 representation 분리
3. issuer identity proof
4. issuer declaration signature
5. canonical representation 주장
6. bridge·IBC 경로 provenance
7. reserve, audit, legal-document pointer
8. fungibility/equivalence 주장
9. redemption·mint·burn reference
10. schema version과 supersession
11. stale, disputed, revoked 상태
12. public field와 restricted field
13. 자산 병합·분리·migration 처리
14. 동일 symbol 충돌 처리
15. chain reorganization 또는 contract migration 영향

## 태그

- `[CANDIDATE] versioned signed Asset Record`
- `[OWNER-Q: BM4-OQ-002] 공개 최소 Asset Record에 반드시 포함할 필드는 무엇인가?`
- `[OWNER-Q: BM4-OQ-003] issuer identity의 허용 증명 방식과 canonical declaration 권한은 어디까지인가?`
- `[OWNER-Q: BM4-OQ-004] reserve·audit·legal attestation을 필수로 요구할 자산 범주가 있는가?`
- `[OWNER-Q: BM4-OQ-005] conflict가 있는 representation을 검색 결과에서 어떻게 노출할 것인가?`
- `[DECISION-PENDING: BM4-DP-002] Minimum public Asset Record and issuer declaration policy`
- `[DEPENDENCY: CH-02] evidence provenance/freshness`
- `[DEPENDENCY: CH-05] capability catalog asset references`
- `[DEPENDENCY: CH-07] issuer, attestation, liability, privacy boundary`

---

# TOPIC 02 — BM4-REG-02 Service Provider Record

## 쉽게 설명

Provider Record는 “이 회사가 좋다”가 아니라 **이 운영 주체가 누구이며 어떤 종류의 서비스를 제공한다고 서명해 선언했는지**를 기록한다.

## 하드코어 범위

Provider identity와 service capability를 분리한다.

- `provider_id`
- operator identity reference
- legal/entity reference if disclosed
- service types: router, relayer, bridge, DEX adapter, gateway, evidence operator, recovery operator 등
- endpoint/reference와 key rotation
- provider signature and delegated signer policy
- terms/policy/jurisdiction references
- service suspension, succession, acquisition, rename
- provider-level incident history와 capability-level incident history 분리

## 세부 항목

1. provider ID와 operator identity
2. legal entity/reference의 선택적 공개
3. signer·key rotation·delegation
4. service-type taxonomy
5. endpoint discovery와 endpoint ownership
6. supported chain/protocol family
7. disclosure jurisdiction/policy pointer
8. contact/security disclosure channel
9. provider status: active, suspended, exited, revoked, unknown
10. corporate succession/merger/migration
11. multi-brand/same-operator linkage
12. evidence operator independence disclosure

## 태그

- `[CANDIDATE] factual Provider Record separate from capability and score`
- `[OWNER-Q: BM4-OQ-006] provider 등록에 legal-entity reference를 필수로 할 범위는 어디까지인가?`
- `[OWNER-Q: BM4-OQ-007] pseudonymous/open-source provider의 진입을 허용할 최소 증명은 무엇인가?`
- `[OWNER-Q: BM4-OQ-008] provider signer delegation과 key-rotation 규칙은 누가 관리하는가?`
- `[DECISION-PENDING: BM4-DP-003] Provider identity and registration minimum`
- `[DEPENDENCY: CH-07] competition, liability, identity and privacy`

---

# TOPIC 03 — BM4-REG-02 Capability Record / Service Catalog

## 쉽게 설명

한 사업자가 모든 체인과 자산을 항상 지원하는 것은 아니다. Capability Record는 **어떤 사업자가 어떤 자산·체인·프로토콜·방향·서비스 등급을 현재 지원한다고 선언하는지**를 세밀하게 기록한다.

## 하드코어 범위

Capability는 provider와 별도 versioned object다.

- `capability_id`, `provider_id`, `service_type`
- supported source/destination chains
- supported assets/representations
- supported protocols and route constraints
- directionality and amount/exposure limits
- service class / SLA template reference
- quote interface and signed quote format
- recovery capabilities and unsupported states
- finality/evidence profile
- capability signature, version, effective/expiry times
- evidence sources, observed-history pointer, bond reference
- self-declared fields and independently observed fields are separate namespaces.

## 세부 항목

1. service type별 mandatory field
2. chain/asset/protocol 지원 matrix
3. source→destination 방향성
4. min/max amount, exposure, rate limits
5. route/path restrictions
6. quote interface/version
7. SLA template and receipt profile
8. finality and evidence profile
9. recovery/refund/return support
10. bond/escrow reference
11. capability version/expiry/revocation
12. planned maintenance and temporary disablement
13. region/policy availability reference
14. observed result history linkage
15. capability inheritance and bundles
16. enterprise service class mapping

## 태그

- `[LOCKED] capability is a factual claim, not a score`
- `[OWNER-Q: BM4-OQ-009] service type별 필수 Capability field를 어디까지 공통화할 것인가?`
- `[OWNER-Q: BM4-OQ-010] amount/exposure limits를 public record에 직접 둘지 reference로 둘지?`
- `[OWNER-Q: BM4-OQ-011] bond reference는 단순 사실 링크인지 eligibility 조건인지?`
- `[OWNER-Q: BM4-OQ-012] BM3가 참조할 service class와 receipt profile의 최소 공통 필드는 무엇인가?`
- `[DECISION-PENDING: BM4-DP-004] Capability schema and service taxonomy`
- `[DEPENDENCY: CH-03] model/version/confidence reference boundary`
- `[DEPENDENCY: CH-04] route, failover, split and recovery capability semantics`
- `[DEPENDENCY: CH-05] structured intent and capability catalog mapping`

---

# TOPIC 04 — Signed Quote and Service Offer References

## 쉽게 설명

Capability가 “평소 제공 가능한 서비스”라면 Signed Quote는 **이번 요청에 대해 얼마, 어떤 경로, 어느 시간까지, 어떤 조건으로 제공하겠다는 구체적 약속**이다.

## 하드코어 범위

Registry는 quote engine을 운영하지 않고 quote schema/reference를 표준화한다.

- request ID and quote ID
- provider/capability version binding
- asset, amount, route-plan reference
- fees, minimum output, expiry
- SLA/policy/recovery references
- provider signature
- quote supersession/cancellation
- quote vs capability consistency checks
- public hash/reference vs private commercial terms boundary

## 세부 항목

1. quote schema version
2. capability binding
3. expiry and stale quote handling
4. quote cancellation/supersession
5. route-plan hash
6. fee/output/finality/recovery disclosure
7. private term redaction and public audit reference
8. quote conflict and replay protection
9. quote history retention
10. enterprise negotiated quote handling

## 태그

- `[CANDIDATE] signed quote reference, not Hub pricing authority`
- `[OWNER-Q: BM4-OQ-013] quote 원문과 hash/reference 중 어떤 수준을 public하게 둘 것인가?`
- `[OWNER-Q: BM4-OQ-014] quote history의 공개 기간과 상업기밀 경계는 무엇인가?`
- `[DECISION-PENDING: BM4-DP-005] Signed Quote publication and retention model`
- `[DEPENDENCY: CH-02] SLA evidence`
- `[DEPENDENCY: CH-05] enterprise request/intent`

---

# TOPIC 05 — BM4-REG-03 Evidence Source and Provenance Model

## 쉽게 설명

같은 사건도 provider API, chain data, indexer, 고객 시스템이 다르게 말할 수 있다. Registry는 **누가 무엇을 관측했고, 원본이 어디 있으며, 서로 얼마나 일치하는지**를 표시해야 한다.

## 하드코어 범위

Evidence is a typed, versioned, provenance-bearing object/reference.

- source class and source identity
- evidence type: declaration, chain proof, tx/ack, indexer observation, provider telemetry, third-party attestation, institutional record
- captured_at, event_time, finalized_at
- signature/hash and verifier
- source independence/correlation
- availability and retention
- confidence, missingness, disagreement
- raw evidence off-chain; minimum hash/pointer may be on-chain
- one indexer or provider self-report cannot be final commercial truth.

## 세부 항목

1. evidence-source taxonomy
2. source independence classification
3. event time vs observation time
4. hash/signature and verifier
5. provenance chain
6. evidence normalization
7. missing field reason codes
8. conflicting evidence sets
9. retention and deletion policy
10. public/private source access
11. evidence quality score versus factual evidence state
12. reproducibility and audit export
13. chain finality profile reference
14. source outage and fallback

## 태그

- `[LOCKED] self-report and independent evidence are distinct`
- `[OWNER-Q: BM4-OQ-015] evidence source hierarchy를 고정 우선순위로 둘 것인가, 사건 유형별 policy로 둘 것인가?`
- `[OWNER-Q: BM4-OQ-016] 상업적 breach 판단에 필요한 최소 독립 corroboration은 무엇인가?`
- `[OWNER-Q: BM4-OQ-017] evidence retention과 접근권한의 기본 기간은?`
- `[DECISION-PENDING: BM4-DP-006] Evidence provenance and corroboration policy`
- `[DEPENDENCY: CH-02] canonical evidence semantics`
- `[DEPENDENCY: CH-07] privacy, disclosure and liability`

---

# TOPIC 06 — BM4-REG-03 Freshness, Missingness, and Confidence

## 쉽게 설명

작년에 맞았던 정보가 오늘도 맞다는 보장은 없다. 그래서 모든 기록에는 **얼마나 최근인지, 무엇이 비어 있는지, 얼마나 확실한지**가 붙어야 한다.

## 하드코어 범위

Freshness is deterministic policy; confidence is bounded evidence/model metadata.

- `observed_at`, `verified_at`, `valid_from`, `expires_at`
- freshness class: CURRENT, AGING, STALE, EXPIRED, UNKNOWN
- service-type-specific freshness windows
- missingness reason and impact
- confidence interval/source agreement
- model confidence is not factual verification
- stale capability may become ineligible only by published rule, not model score.

## 세부 항목

1. asset/issuer record freshness
2. provider identity freshness
3. capability heartbeat/renewal
4. evidence-source freshness
5. incident update freshness
6. bond/escrow reference freshness
7. missingness taxonomy
8. confidence interval and abstention
9. stale-data UX
10. refresh failure and grace period
11. clock/source inconsistency
12. version-binding and rollback

## 태그

- `[CANDIDATE] deterministic freshness states`
- `[OWNER-Q: BM4-OQ-018] service type별 freshness window를 누가 정하고 갱신하는가?`
- `[OWNER-Q: BM4-OQ-019] stale 상태가 자동 eligibility failure가 되는 최소 범위는?`
- `[DECISION-PENDING: BM4-DP-007] Freshness windows and stale-data effects`
- `[DEPENDENCY: CH-02] timestamp and evidence rules`

---

# TOPIC 07 — BM4-REG-03 Incident Lifecycle and Disclosure

## 쉽게 설명

사고가 있었다는 사실만으로 영구 퇴출하거나, 반대로 현재 정상이라는 이유로 과거 사고를 지우면 안 된다. Registry는 **무슨 사고가 어디까지 영향을 줬고, 어떻게 복구됐으며, 아직 무엇이 미해결인지**를 기록한다.

## 하드코어 범위

Incident object and lifecycle:

```text
REPORTED → TRIAGED → CONFIRMED / DISPUTED
→ MITIGATING → RECOVERED / PARTIALLY_RECOVERED
→ CLOSED / UNRESOLVED / SUPERSEDED
```

Fields include incident ID, affected provider/capability/routes/assets, event window, source/evidence, severity, controllability, last-known asset location, recovery actions, resolution, compensation reference if separately authorized, and disclosure status.

## 세부 항목

1. incident taxonomy
2. severity and affected scope
3. provider-controlled vs external event
4. report source and corroboration
5. dispute state
6. mitigation and recovery actions
7. customer-impact aggregation
8. disclosure timing and embargo
9. remediation evidence
10. recurrence linkage
11. closure criteria
12. unresolved and unknown state
13. legal/compensation reference separation

## 태그

- `[LOCKED] incident fact does not equal legal fault`
- `[OWNER-Q: BM4-OQ-020] incident severity와 public disclosure threshold는 어떻게 정할 것인가?`
- `[OWNER-Q: BM4-OQ-021] 보안 취약점·포렌식 정보의 embargo와 공개 전환 권한은 누구에게 있는가?`
- `[OWNER-Q: BM4-OQ-022] provider-controlled/external/unresolved 분류의 최종 review 주체는?`
- `[DECISION-PENDING: BM4-DP-008] Incident lifecycle, disclosure and closure policy`
- `[DEPENDENCY: CH-02] evidence and recovery status`
- `[DEPENDENCY: CH-04] last-known asset location and recovery state`
- `[DEPENDENCY: CH-07] liability and disclosure`

---

# TOPIC 08 — BM4-REG-03 Revocation, Suspension, Correction, and Appeal

## 쉽게 설명

잘못된 키, 만료된 증거, 허위 선언, 서비스 종료가 있으면 기록을 멈추거나 취소해야 한다. 다만 누가든 임의로 퇴출할 수 없도록 **사유, 증거, 기간, 이의제기 절차**가 필요하다.

## 하드코어 범위

Separate object-level status from provider-level market exclusion.

- declaration revocation
- capability suspension/revocation
- signer/key compromise
- evidence invalidation
- emergency temporary hold
- correction and supersession
- issuer/provider voluntary withdrawal
- appeal/review and audit trail
- revocation does not delete historical records.

## 세부 항목

1. voluntary withdrawal
2. expiry vs revocation
3. emergency suspension
4. key compromise
5. false/misleading declaration
6. evidence invalidation
7. correction/supersession
8. review/appeal
9. reinstatement
10. historical retention
11. cross-object cascade rules
12. governance emergency powers

## 태그

- `[CANDIDATE] history-preserving revocation`
- `[OWNER-Q: BM4-OQ-023] emergency suspension 권한과 최대 유효기간은?`
- `[OWNER-Q: BM4-OQ-024] issuer/provider의 appeal 및 reinstatement 절차는?`
- `[OWNER-Q: BM4-OQ-025] 한 capability revocation이 provider 전체에 전파되는 조건은?`
- `[DECISION-PENDING: BM4-DP-009] Revocation authority, cascade and appeal model`
- `[DEPENDENCY: CH-07] governance and due-process boundary`

---

# TOPIC 09 — BM4-REG-04 Deterministic Eligibility

## 쉽게 설명

Eligibility는 “좋아 보인다”가 아니라 **서비스 후보 목록에 들어가기 위한 최소 객관 조건을 충족했는가**다.

## 하드코어 범위

Eligibility is deterministic, published, versioned, and service-specific.

Possible rules:

- valid provider signature and active identity
- active non-expired capability
- required evidence fields present
- supported asset/route/protocol match
- policy/allowlist match
- quote valid and internally consistent
- required bond/reference present where applicable
- no active hard suspension
- data freshness above minimum
- amount/exposure within limits

Eligibility produces pass/fail/reason codes. It does not rank eligible providers.

## 세부 항목

1. service-specific rule sets
2. mandatory vs optional fields
3. evidence minimum
4. freshness threshold
5. policy/allowlist compatibility
6. quote consistency
7. incident/suspension effect
8. bond reference effect
9. deterministic reason codes
10. fail-closed and UNKNOWN treatment
11. rule versioning
12. appeal and exception prohibition/handling

## 태그

- `[LOCKED] eligibility separate from ranking`
- `[OWNER-Q: BM4-OQ-026] 각 service type의 최소 eligibility rule을 어디까지 공통화할 것인가?`
- `[OWNER-Q: BM4-OQ-027] bond 또는 independent evidence를 필수 eligibility로 둘 서비스 범주는?`
- `[OWNER-Q: BM4-OQ-028] UNKNOWN/missing 상태를 fail, hold, limited로 처리할 기준은?`
- `[DECISION-PENDING: BM4-DP-010] Deterministic eligibility policy`
- `[DEPENDENCY: CH-05] institutional policy matching`
- `[DEPENDENCY: CH-07] non-discrimination and liability`

---

# TOPIC 10 — BM4-REG-04 Ranking, Confidence, and Advisory Selection

## 쉽게 설명

여러 provider가 최소 조건을 모두 통과했다면 사용자는 비용, 속도, 복구 이력 등을 보고 선택할 수 있다. Ranking은 **선택을 돕는 의견**이지 자동 승인이나 퇴출 명령이 아니다.

## 하드코어 범위

- ranking inputs: price, output, latency distribution, completion/recovery history, evidence quality, concentration effect, user policy
- deterministic comparator and model/advisory ranking are labeled separately
- model/version, feature time, confidence interval, missingness, abstention
- high rank ≠ endorsement; low rank ≠ ineligibility
- user/institution may choose or set deterministic weights
- audit and replay of ranking output
- anti-feedback-loop and provider concentration controls

## 세부 항목

1. deterministic weighted ranking
2. model-assisted ranking
3. confidence and abstention
4. explanation and reason codes
5. missing-data discount
6. self-report discount
7. personalization vs public ranking
8. institution policy weights
9. ranking history and reproducibility
10. feedback-loop monitoring
11. anti-gaming
12. no default mandatory provider

## 태그

- `[LOCKED] ranking cannot grant approval or automatic exclusion`
- `[OWNER-Q: BM4-OQ-029] Registry가 기본 ranking을 제공할지, provider/wallet별 ranking만 허용할지?`
- `[OWNER-Q: BM4-OQ-030] public ranking에 포함 가능한 지표와 금지할 지표는?`
- `[OWNER-Q: BM4-OQ-031] model-assisted rank의 공개·감사·abstention 요건은?`
- `[DECISION-PENDING: BM4-DP-011] Ranking surface and advisory authority`
- `[DEPENDENCY: CH-03] AI model/version/confidence`
- `[DEPENDENCY: CH-05] user/institution policy`

---

# TOPIC 11 — BM4-REG-05 Open Entry and Newcomer Evaluation

## 쉽게 설명

과거 실적이 많은 기존 사업자만 유리하면 시장이 고착된다. 새 provider도 **안전한 소규모 범위에서 검증받고 성장할 수 있는 진입 경로**가 필요하다.

## 하드코어 범위

- open schema and non-exclusive registration
- staged capability status: declared → verified subset → bounded eligible → general eligible
- newcomer exploration/evaluation quota or sandbox
- capped amount/exposure and enhanced evidence requirements
- history scarcity explicitly shown, not converted to “bad provider”
- bond/attestation options without making capital barrier discriminatory
- anti-sybil and related-operator disclosure

## 세부 항목

1. registration process
2. capability declaration test
3. sandbox/bounded evaluation
4. amount/exposure caps
5. evidence requirements
6. newcomer display label
7. history scarcity treatment
8. bond alternatives
9. anti-sybil/related operator
10. graduation criteria
11. failure and exit handling
12. fee neutrality

## 태그

- `[LOCKED] open entry and no exclusive mandatory operator`
- `[OWNER-Q: BM4-OQ-032] newcomer evaluation을 quota, sandbox, random exploration 중 어떻게 설계할 것인가?`
- `[OWNER-Q: BM4-OQ-033] newcomer의 initial exposure cap과 graduation 기준은?`
- `[OWNER-Q: BM4-OQ-034] anti-sybil을 위해 요구할 identity/economic proof의 한계는?`
- `[DECISION-PENDING: BM4-DP-012] Open-entry and newcomer policy`
- `[DEPENDENCY: CH-07] competition and discrimination`

---

# TOPIC 12 — BM4-REG-05 Switching, Portability, and Exit

## 쉽게 설명

한 provider가 불편하거나 위험해졌을 때 사용자가 쉽게 다른 provider로 옮길 수 있어야 한다. Switching은 시장 경쟁의 실제 작동 여부를 보여준다.

## 하드코어 범위

- portable capability/quote/receipt schemas
- no proprietary mandatory client or data lock-in
- exportable history and evidence references
- route/provider substitution before authorization
- enterprise contract and credential portability boundary
- switching friction measurement
- provider exit and successor handling

## 세부 항목

1. schema portability
2. API compatibility
3. receipt/history export
4. credential/config migration
5. provider exit notification
6. capability successor
7. contract lock-in visibility
8. switching cost/time
9. route substitution
10. user policy migration
11. data retention after exit
12. emergency switching

## 태그

- `[CANDIDATE] measurable switching and portability`
- `[OWNER-Q: BM4-OQ-035] Registry가 요구할 최소 portability/API 호환 범위는?`
- `[OWNER-Q: BM4-OQ-036] switching friction 공개 KPI를 어떤 단위로 측정할 것인가?`
- `[DECISION-PENDING: BM4-DP-013] Switching and portability requirements`
- `[DEPENDENCY: CH-05] gateway portability`

---

# TOPIC 13 — BM4-REG-05 Concentration, Dominance, and Neutrality KPI

## 쉽게 설명

가장 높은 점수를 받은 provider에게 거래가 계속 몰리면 점점 더 많은 데이터와 실적을 쌓아 독점이 강화될 수 있다. 그래서 시장 집중도를 계속 측정해야 한다.

## 하드코어 범위

- top-1/top-3 share
- HHI or equivalent concentration measure
- quote coverage and spread
- route/asset/chain segment concentration
- model-provider and evidence-source concentration
- related-operator aggregation
- switching and newcomer opportunities
- concentration alerts and policy response
- no automatic forced redistribution without explicit policy.

## 세부 항목

1. provider share by volume/count/revenue
2. route-specific concentration
3. asset/chain concentration
4. evidence-source concentration
5. model/ranking-provider concentration
6. related entity aggregation
7. quote spread
8. switching rate
9. newcomer exposure
10. concentration trend
11. alert threshold
12. permitted mitigation

## 태그

- `[LOCKED] concentration must be measured`
- `[OWNER-Q: BM4-OQ-037] concentration KPI는 어떤 지표와 기간으로 운영할 것인가?`
- `[OWNER-Q: BM4-OQ-038] alert threshold를 넘을 때 가능한 대응은 경고, exploration 확대, eligibility 제한 중 어디까지인가?`
- `[DECISION-PENDING: BM4-DP-014] Concentration thresholds and response policy`
- `[DEPENDENCY: CH-07] competition policy`

---

# TOPIC 14 — BM4-REG-06 Conflict Detection Taxonomy

## 쉽게 설명

한 자산에 대해 서로 다른 원본 주장이 나오거나, provider가 지원한다고 했지만 quote는 다른 조건을 말할 수 있다. Registry는 먼저 **무엇이 충돌했는지 정확히 분류**해야 한다.

## 하드코어 범위

Conflict classes:

- asset identity/canonical representation conflict
- issuer/signature conflict
- capability-version conflict
- capability vs quote conflict
- stale evidence vs active capability conflict
- incident/revocation conflict
- provider claims vs independent observation
- policy/capability incompatibility
- model disagreement beyond confidence threshold
- related-operator or concentration conflict

Each conflict has signed inputs, schema/version, detected_at, deterministic rule set, status, and audit trail.

## 세부 항목

1. object-identity conflict
2. version conflict
3. signature/authority conflict
4. semantic field conflict
5. freshness conflict
6. quote/capability conflict
7. evidence disagreement
8. incident/revocation disagreement
9. policy mismatch
10. concentration conflict
11. duplicate record
12. unresolved/unknown conflict

## 태그

- `[CANDIDATE] explicit conflict object and taxonomy`
- `[OWNER-Q: BM4-OQ-039] 어떤 conflict는 자동 탐지·차단하고 어떤 conflict는 경고만 할 것인가?`
- `[OWNER-Q: BM4-OQ-040] conflict 공개 범위와 sensitive evidence redaction 기준은?`
- `[DECISION-PENDING: BM4-DP-015] Conflict taxonomy and detection effects`
- `[DEPENDENCY: CH-02, CH-05, CH-07]`

---

# TOPIC 15 — BM4-REG-06 Deterministic Arbitration and Unresolved State

## 쉽게 설명

충돌이 생겼을 때 AI가 몰래 승자를 고르는 것이 아니라, **공개된 우선순위 규칙을 적용하고 그래도 풀리지 않으면 미해결 상태로 남겨야 한다.**

## 하드코어 범위

Processing:

```text
signed inputs
→ schema validation
→ signature/authority validation
→ version and freshness validation
→ deterministic priority rule
→ resolved / partially resolved / unresolved / fail-closed
→ audit record and review path
```

Possible priorities are not globally fixed yet; they may include explicit supersession, cryptographic authority, newer valid version, independent corroboration, scope-specific policy, or fail-closed. Human/governance review must not silently rewrite evidence.

## 세부 항목

1. priority-rule version
2. signed input binding
3. scope-specific rules
4. fail-closed conditions
5. partial resolution
6. unresolved display
7. pause/review authority
8. appeal and new evidence
9. audit trail
10. rule change governance
11. anti-bias review
12. no hidden super-agent

## 태그

- `[LOCKED] deterministic public arbitration; no unrestricted super-agent`
- `[OWNER-Q: BM4-OQ-041] conflict 우선순위 원칙을 cryptographic authority, freshness, independent corroboration 중 어떤 순서로 둘 것인가?`
- `[OWNER-Q: BM4-OQ-042] unresolved 상태에서 서비스 검색·eligibility·execution plan을 fail-closed할 범위는?`
- `[OWNER-Q: BM4-OQ-043] pause/review 최종 권한과 appeal 절차는?`
- `[DECISION-PENDING: BM4-DP-016] Arbitration priority and unresolved-state policy`
- `[PROJECT-OWNER-Q: OR-03]`

---

# TOPIC 16 — Public/on-chain vs Off-chain/Restricted Data Boundary

## 쉽게 설명

검증에 필요한 최소 정보는 공개할 수 있지만, 개인정보·기관 정책·영업비밀·상세 사고 자료를 모두 체인에 올리면 안 된다.

## 하드코어 범위

Potential public/on-chain minimum:

- stable identifiers
- signature and schema version
- capability hash/minimum fields
- evidence pointer/freshness
- quote/SLA/bond/receipt references
- incident/revocation status
- final recovery status

Off-chain/access controlled:

- raw KYC/PII
- detailed institution policy
- raw high-frequency telemetry
- proprietary features/models
- private commercial terms
- unreleased vulnerability and forensic detail

Data minimization, retention, encryption, redaction, access log, deletion/legal hold, and hash-linkability risks must be specified.

## 태그

- `[LOCKED] no raw KYC/PII or sensitive policy on public chain`
- `[OWNER-Q: BM4-OQ-044] public minimum record를 어느 수준까지 두고 나머지는 어떤 access model로 관리할 것인가?`
- `[OWNER-Q: BM4-OQ-045] public hash/pointer가 민감정보를 역추론하게 할 위험을 어떻게 제한할 것인가?`
- `[DECISION-PENDING: BM4-DP-017] Data placement and access-control model`
- `[DEPENDENCY: CH-07] privacy and legal retention`

---

# TOPIC 17 — Query, Discovery, API, and User Experience

## 쉽게 설명

사용자는 “USDC를 이 체인에서 저 체인으로 보내는 서비스를 누가 지원하는가?”를 검색할 수 있어야 한다. 결과에는 지원 여부뿐 아니라 증거 시점과 부족한 정보도 보여야 한다.

## 하드코어 범위

- query by asset, chain, route, protocol, service type, service class, evidence freshness, incident/revocation state
- deterministic eligibility filter
- ranking optional and clearly labeled
- signed response or verifiable snapshot
- pagination/rate limits/caching
- schema negotiation and versioning
- historical query and audit export
- no misleading badge or hidden sponsored ranking

## 세부 항목

1. discovery API
2. exact and fuzzy asset search
3. capability filter
4. eligibility filter
5. ranking interface
6. evidence/freshness display
7. missingness/conflict display
8. history query
9. audit export
10. rate limits
11. schema version negotiation
12. wallet/enterprise UX
13. sponsored result disclosure
14. accessibility/localization

## 태그

- `[CANDIDATE] neutral query and discovery interface`
- `[OWNER-Q: BM4-OQ-046] Registry 자체 ranking UI를 제공할지 factual search만 제공할지?`
- `[OWNER-Q: BM4-OQ-047] public free API와 paid enterprise feed의 경계는?`
- `[DECISION-PENDING: BM4-DP-018] Query/API and UX surface`
- `[DEPENDENCY: CH-05] enterprise catalog and intent mapping`

---

# TOPIC 18 — Security, Abuse, Sybil, and Data-Poisoning Threat Model

## 쉽게 설명

공급자가 허위 지원 정보를 올리거나, 공격자가 provider 계정을 가로채거나, 가짜 실적으로 점수를 조작할 수 있다. Registry는 이런 공격을 전제로 설계해야 한다.

## 하드코어 범위

Threats:

- key compromise and unauthorized update
- sybil providers and related-operator concealment
- false capability/quote
- telemetry/data poisoning
- incident suppression
- replay and stale-record attack
- evidence-source collusion
- ranking manipulation and wash activity
- denial of service and censorship
- privacy inference
- governance capture

Controls include signed versioned updates, rotation/revocation, independent corroboration, anomaly flags, rate limiting, related-entity disclosure, audit trails, and fail-closed rules.

## 태그

- `[CANDIDATE] explicit threat model before MVP`
- `[OWNER-Q: BM4-OQ-048] anti-sybil과 open entry 사이의 최소 균형 기준은?`
- `[OWNER-Q: BM4-OQ-049] 허위 capability·telemetry에 대한 제재를 Registry 상태, bond, 법적 절차 중 어디까지 연결할 것인가?`
- `[DECISION-PENDING: BM4-DP-019] Security and anti-gaming control set`
- `[DEPENDENCY: CH-03, CH-07]`

---

# TOPIC 19 — Legal, Liability, Attestation, and Claim Language

## 쉽게 설명

Registry에 정보가 있다고 해서 Hub가 안전성이나 법률 준수를 보증하는 것으로 오해되면 안 된다. 누가 정보를 냈고 누가 검증했으며 Registry는 무엇을 하지 않는지가 명확해야 한다.

## 하드코어 범위

- listing vs verification vs attestation vs certification separation
- issuer/provider/evidence operator/registry operator responsibility matrix
- no safe/compliant/guaranteed implication
- jurisdiction/policy reference as disclosed fact only
- incident and fault distinction
- dispute/appeal/due process
- terms of use, reliance, limitation, audit and record-retention boundary
- commercial SLA/compensation is outside current authorization.

## 태그

- `[LOCKED] no regulatory-compliance or guarantee badge`
- `[OWNER-Q: BM4-OQ-050] Registry operator의 책임 범위와 reliance disclaimer를 어떤 수준으로 둘 것인가?`
- `[OWNER-Q: BM4-OQ-051] third-party attestation의 인정·철회·책임 기준은?`
- `[DECISION-PENDING: BM4-DP-020] Legal responsibility and claim-control model`
- `[DEPENDENCY: CH-07] direct owner`

---

# TOPIC 20 — Fees, Revenue, and Economic Sustainability

## 쉽게 설명

Registry가 운영되려면 비용이 든다. 다만 base IBC에 통행료를 강제로 붙이거나 특정 provider를 밀어주는 방식은 금지된다. 가능한 수익은 등록·검증·기업용 데이터·감사 서비스처럼 선택적이어야 한다.

## 하드코어 범위

Candidate revenue surfaces:

- optional registration/update fees
- evidence verification/attestation processing fees
- enterprise API/feed subscription
- audit export and managed integration
- dispute/appeal processing with anti-abuse design
- premium freshness/monitoring services operated competitively

Need cost model for storage, indexing, evidence reconciliation, security, governance, and support. Fees must not become mandatory base-IBC toll or closed-entry barrier.

## 태그

- `[LOCKED] no forced Hub toll on base IBC; no mandatory ATOM payment`
- `[OWNER-Q: BM4-OQ-052] Registry의 우선 수익면은 registration, verification, enterprise feed 중 무엇인가?`
- `[OWNER-Q: BM4-OQ-053] 무료 공개 데이터와 유료 서비스의 분리 원칙은?`
- `[OWNER-Q: BM4-OQ-054] fee가 newcomer 진입장벽이 되지 않도록 할 정책은?`
- `[DECISION-PENDING: BM4-DP-021] Registry fee and revenue model`
- `[DEPENDENCY: CH-01] revenue attribution and protocol share`
- `[DEPENDENCY: CH-07] economics and competition`

---

# TOPIC 21 — Governance, Schema Evolution, and Operator Model

## 쉽게 설명

자산·프로토콜·증거 형식은 계속 변한다. 스키마를 바꿀 때 기존 기록을 깨뜨리지 않고, 누가 변경할 수 있는지 공개해야 한다.

## 하드코어 범위

- schema registry and semantic versioning
- backward compatibility
- migration and deprecation
- rule-set version binding
- emergency patch vs normal governance
- multi-operator federation or single reference operator
- open-source reference implementation
- audit/change log
- no silent eligibility/ranking rule mutation

## 태그

- `[CANDIDATE] versioned public schemas and rules`
- `[OWNER-Q: BM4-OQ-055] schema/rule change 권한을 governance, technical committee, multi-operator consensus 중 어디에 둘 것인가?`
- `[OWNER-Q: BM4-OQ-056] emergency patch와 정상 변경의 승인·유효기간은?`
- `[DECISION-PENDING: BM4-DP-022] Governance and schema-evolution model`
- `[DEPENDENCY: CH-00, CH-07]`

---

# TOPIC 22 — Cross-channel Interfaces and Shared Objects

## 쉽게 설명

BM4는 혼자 동작하지 않는다. BM2의 증거·SLA, BM3의 intent·catalog, failover 채널의 recovery 정보 등을 받아 공통 객체로 연결해야 한다.

## 하드코어 범위

- CH-01: distribution provider role, campaign performance, revenue attribution
- CH-02: evidence, timestamps, SLO/history, incident semantics
- CH-03: model confidence/version and non-eligibility boundary
- CH-04: route/failover/split capability, unique ID, recovery, asset location
- CH-05: structured intent, policy profile, service class, receipt profile
- CH-07: competition, listing/verification/liability/privacy/fees
- CH-00: common object promotion and Owner decisions

Shared-object changes require structured dependency requests; CH-06 must not edit other channel files.

## 태그

- `[LOCKED] no silent cross-channel object redefinition`
- `[OWNER-Q: BM4-OQ-057] Asset/Provider/Capability 중 어떤 객체를 CH-00 공통 객체로 우선 승격할 것인가?`
- `[DECISION-PENDING: BM4-DP-023] Shared-object integration sequence`
- `[DEPENDENCY: CH-00 through CH-07]`

---

# TOPIC 23 — CosmWasm MVP Candidate, Phasing, and Gates

## 쉽게 설명

처음부터 거대한 native module을 만들지 않는다. 먼저 작은 스키마·등록·조회·취소 기능과 오프체인 증거 연결을 시험한다.

## 하드코어 범위

Candidate sequence:

```text
schema and examples
→ off-chain reference registry/prototype
→ signed record validation
→ freshness/revocation and conflict tests
→ minimal audited CosmWasm record/reference MVP
→ bounded provider/asset set
→ evidence, neutrality, security and economic evaluation
→ native module only after separately proven bottleneck and Owner authorization
```

MVP candidates:

- Asset Record minimum
- Provider/Capability record minimum
- version/supersession/revocation
- evidence pointer/freshness
- deterministic eligibility reason codes
- query/export reference
- no ranking monopoly, custody, execution, compensation or PII.

## 태그

- `[LOCKED] contracts/data/CosmWasm before native module`
- `[OWNER-Q: BM4-OQ-058] MVP의 최초 asset/provider/chain/service universe는?`
- `[OWNER-Q: BM4-OQ-059] 최초 MVP에 eligibility까지 포함할지 factual records만 포함할지?`
- `[OWNER-Q: BM4-OQ-060] MVP operator와 independent evidence source 후보는?`
- `[DECISION-PENDING: BM4-DP-024] Bounded MVP scope and gate sequence`
- `[HOLD] implementation is not currently authorized`

---

# TOPIC 24 — KPI, Validation, Hold/Kill, and Claim Ceiling

## 쉽게 설명

Registry가 성공하려면 기록 수가 많기만 해서는 안 된다. 정보가 최신이고 재현 가능하며 provider를 바꿀 수 있고 독점이 심해지지 않는지를 측정해야 한다.

## 하드코어 범위

Candidate KPIs:

- required-field and provenance coverage
- freshness and stale rate
- independent corroboration rate
- conflict and unresolved rate
- incident/revocation resolution time
- active independent providers
- comparable quote coverage and spread
- switching rate/friction
- newcomer evaluation/graduation
- top-provider/evidence-source/model concentration
- query reproducibility and audit-export success
- false/misleading label count
- PII/private-data leakage incidents
- operating cost and external revenue

Validation remains affected-scope only. Current pre-PoC claim ceiling is C2. No channel readback or Git write creates validation PASS.

## 태그

- `[LOCKED] no global validation loop`
- `[LOCKED] C2 maximum before PoC`
- `[OWNER-Q: BM4-OQ-061] BM4-REG-01~06 closure에 필요한 정량 KPI threshold는?`
- `[DECISION-PENDING: BM4-DP-025] KPI and promotion gate set`
- `[PROJECT-OWNER-Q: OR-09]`

---

# Execution order

```text
BM4-REG-01 Asset / issuer schema
→ BM4-REG-02 Provider / capability schema
→ BM4-REG-03 Evidence / freshness / incident / revocation
→ BM4-REG-04 Eligibility / ranking / confidence
→ BM4-REG-05 Open entry / switching / concentration
→ BM4-REG-06 Conflict detection / deterministic arbitration
→ cross-channel common objects
→ bounded MVP decision only after separate authorization
```

# Response footer template

Every substantive response appends:

```text
[CH-06 TOPIC INDEX]
CURRENT_TOPIC =
EASY_EXPLANATION_COMPLETE =
HARDCORE_DETAIL_COMPLETE =
STATUS = LOCKED / CANDIDATE / OPEN / HOLD / REJECTED
OWNER_QUESTIONS_OPEN =
DECISION_POINTS_PENDING =
CURRENT_DECISION_RECORDS = BM4-REG-D-0001 / 0002 / 0003
DEPENDENCIES =
MEMORY_UPDATE = NONE / CHAT_ONLY / GIT_CANDIDATE / MERGED
NEXT_EXACT_ACTION =
```
