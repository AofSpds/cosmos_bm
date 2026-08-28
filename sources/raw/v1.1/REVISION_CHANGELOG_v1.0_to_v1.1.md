# COSMOS HUB BM 개선 제안서 v1.0 → v1.1 Candidate 변경이력

## 1. 개정 범위

- 기준 문서: `COSMOS HUB BM 개선 제안서 v1.0 / 2026-08-27`
- 개정 문서: `COSMOS HUB BM 개선 제안서 v1.1 CANDIDATE / 2026-08-28`
- 개정 방식: 기존 중심 명제와 4개 BM을 유지한 제한적 보정
- 유지한 핵심: Thin Core, Rich Edges / 기본 IBC 강제 통행료 금지 / 고객 원금 비수탁 / 4개 BM 순서 / CosmWasm 우선·native module 후행 / ATOM 강제 결제 금지
- 미수행 범위: 신규 BM 추가, Hub native DEX·EVM·lending·privacy 확장, CCP·netting 기능 추가, 전면 재작성

## 2. 주요 명칭 변경

| v1.0 | v1.1 Candidate |
|---|---|
| Neutral Interchain Clearing Market | Neutral Interchain Coordination Market |
| Guaranteed Interchain Delivery | Assured Interchain Delivery SLA |
| Guaranteed Delivery Market | Delivery Assurance Market |
| guarantee | assurance / SLA-backed compensation |
| clearing fee | coordination / protocol fee |

NICM 약어는 유지했다. SWIFT·VisaNet·CLS·IX 비교에는 기능적 비유일 뿐 법률상 청산기관·CCP·지급결제기관·보험자·원금보증기관을 의미하지 않는다는 제한문을 추가했다.

## 3. P0 반영 내역

| 항목 | 반영 위치 | 변경 내용 |
|---|---|---|
| Injective USDC 증거강도 보정 | Executive Summary, §1.3, §4.4, §8.3, 부록 A, R3·R12 | 실현 반복매출이 아닌 `CONTRACTED / PUBLICLY ANNOUNCED / ROLLOUT IN PROGRESS / REPEATED ON-CHAIN REVENUE NOT YET VERIFIED` 상태로 분리 |
| Eureka 접근·relay 분리 | §1.1, §1.2 역할분담표, §10.3, 부록 A, R8 | permissionless access와 초기 permissioned relay set, relay liveness 의존성을 분리 |
| 실패·복구 모델 현실화 | §3.3, §5.1~§5.3, §10.3, Technical MVP 산출물, 부록 B, R21 | 보편적 automatic revert를 제거하고 source 환불, swap-chain 잔류, intermediate-chain 잔류, 수동복구 등 경로별 상태를 추가 |
| 법률상 과대표현 완화 | 표지, §2.2, §3.1, §5 전체, §11.3, 도식 1·2 | Clearing→Coordination, Guaranteed→Assured SLA로 변경; 고객원금·체인 finality 보증 및 무근거 insurance 표현 금지 |
| 기관계약 당사자·수익집행 | §6.4, §11.3, §14.3, 리스크표 | 기존 운영법인·중립 SPV/협회·복수 사업자 라이선스 모델 비교와 표준 라이선스 10개 필수조항 추가 |

## 4. P1 반영 내역

| 항목 | 반영 위치 | 변경 내용 |
|---|---|---|
| Revenue Vault 워터폴 | §8.2~§8.3, 도식 3 | Gross Revenue→provider·비용 공제→Operating Floor→Assurance Reserve→Security Budget→Residual Allocation 순서로 변경 |
| 50/30/20의 지위 변경 | §8.3 | 준비금 목표를 충족한 잔여 순수익에만 적용하는 pilot illustration로 하향 |
| Provider Bond 담보정책 | §5.2, §10.3.1, 리스크표 | 안정자산 1차 담보, ATOM haircut, mark-to-market, top-up, 경로·사업자 노출한도와 wrong-way risk 추가 |
| Distribution anti-gaming | §4.2.1, §4.3~§4.4, §12.2 | baseline 대비 incremental time-weighted balance, 30·60·90일 retention, 관계주소·wash transfer 제외, 후지급·clawback, 계산코드 버전 공개 추가 |
| Issuer badge 제한 | §7.2~§7.3, 부록 B | Issuer Signature Verified 등 사실확인형 레이블만 허용하고 Hub Approved·Safe Asset·Regulatory Compliant 등 금지 |
| ATOM 매입 집행정책 | §8.5 | TWAP/batch auction, 한도, slippage cap, venue 경쟁, MEV 보호, 이해상충, 사후공개, Community Pool 입금 증거 규칙 추가 |

## 5. P2 및 문서 정비 내역

| 항목 | 반영 내용 |
|---|---|
| 버전·표지 | `v1.1 CANDIDATE`, 개정일 `2026-08-28`, 개정 성격 표기 |
| 변경이력 | 표지 뒤 별도 변경이력 페이지 추가 |
| 도식 | Coordination 명칭, Eureka transport dependency, Recovery State, 위험기반 수익 워터폴로 3개 도식 교체 |
| 레퍼런스 | R3·R8 활용설명 확장, R21 `Cross-chain Failure Cases` 추가 |
| 상시문서 고정정보 | 확인일, 인용 섹션, 게시 버전/commit 표시 여부, archive/PDF 보존 여부 병기 |
| 용어집 | Coordination, Settlement/Recovery Receipt, Assurance, Recovery State 정의 보강 |
| Revenue Dashboard | Contracted / Accrued / Received / ATOM Purchased / Community Pool Deposited / Pending·Overdue 상태 분리 |
| 90일 산출물 | Customer Evidence, Legal Boundary, Technical MVP, Revenue Dashboard 필수내용 확대 |

## 6. 구조 보존 확인

- 기존 4개 BM 순서와 장별 논리구조를 유지했다.
- 원본 텍스트 블록의 약 82.8%가 exact match로 보존됐으며, 변경은 지정된 보정 문단·표·도식 및 신규 필수 절에 집중됐다.
- DOCX 최종 렌더링은 A4 24페이지이며, 표·도식·상호참조의 페이지 잘림이나 겹침이 없도록 조정했다.
