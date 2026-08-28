# CROSS-VALIDATION CLOSURE NOTE

## 1. 수정항목별 반영 위치 및 반영 여부

| 수정항목 | 반영 위치 | 상태 |
|---|---|---|
| Injective USDC 증거강도 하향 | Executive Summary, §1.3, §4.4, §8.3, 부록 A, R3·R12 | 반영 완료 |
| 계약·롤아웃·수령·ATOM 매입·Pool 귀속 구분 | §1.3 Evidence Status, §8.4, §14.1·§14.3 Revenue Dashboard | 반영 완료 |
| Eureka permissionless access / permissioned relay 분리 | §1.1, §1.2, §10.3, 부록 A, R8 | 반영 완료 |
| automatic revert 제거 및 failure taxonomy | §3.3, §5.1~§5.3, §10.3, 부록 B, R21 | 반영 완료 |
| Settlement/Recovery Receipt 상태 확장 | §3.3, §5.3, Technical MVP Spec | 반영 완료 |
| Clearing→Coordination | 표지, 본문, 표·도식·부록·헤더 | 반영 완료 |
| Guaranteed→Assured SLA | Executive Summary, BM2, 표·도식·부록 | 반영 완료 |
| 법률상 청산·보증·보험 과대해석 제한 | §2.2, §3.1, §11.3 | 반영 완료 |
| 기관계약 당사자 3모델 비교 | §6.4 | 반영 완료 |
| protocol share 강제·감사·연체·회피 처리 | §6.4 표준 라이선스, §13 리스크 | 반영 완료 |
| 고정 50/30/20→위험기반 waterfall | §8.2~§8.3, 도식 3 | 반영 완료 |
| Provider Bond 안정자산·ATOM haircut·wrong-way risk | §5.2, §10.3.1, §13 | 반영 완료 |
| Distribution attribution anti-gaming | §4.2.1, §4.3~§4.4, §12.2 | 반영 완료 |
| issuer badge 범위 제한 | §7.2~§7.3 | 반영 완료 |
| ATOM Buyback Execution Policy | §8.5 | 반영 완료 |
| R3·R8 활용설명 및 R21 | 부록 C | 반영 완료 |
| 변경이력·v1.1 Candidate 표기 | 표지, 변경이력 페이지, 헤더 | 반영 완료 |
| DOCX/PDF 렌더링 | A4 24페이지 전체 | 반영 완료 |

## 2. 남은 오픈 이슈

- 90일 Discovery에서 최종 계약 법인모델을 선택해야 한다.
- 발행사·기관·provider의 실제 willingness-to-pay, bond 제공 의사 및 recovery support 의사를 확보해야 한다.
- Assurance Reserve의 수치 목표와 경로·provider별 exposure cap을 실제 손실·거래자료로 보정해야 한다.
- Revenue Vault와 buyback 집행자의 권한·키 관리·회계 운영절차를 확정해야 한다.
- CosmWasm MVP의 admin·pause·upgrade·migration 주체를 확정해야 한다.

## 3. 외부 법률검토가 필요한 항목

- 계약 당사자, invoice 발행, 세금·회계처리 및 protocol share의 법적 집행방식
- custody, money transmission, payment-system 및 암호자산서비스 규제 경계
- SLA compensation과 provider bond가 보험 또는 보증으로 분류되는 조건
- AML·제재·국가별 접근통제 책임의 배분
- Hub-certified 또는 후속 인증표장의 상표·책임·정지 절차
- 사고 손해배상 한도, 분쟁해결, 준거법과 관할
- Revenue Vault의 ATOM 매입·Community Pool 귀속에 대한 거버넌스·세무·시장집행 경계

## 4. 실제 온체인 수익 검증이 필요한 항목

- Injective USDC 관련 공개 계약 또는 약정의 원문·최종 조건
- Contracted Revenue와 Accrued Revenue의 실제 발생
- Cash/Token Received의 반복 입금과 수령 주소
- 실제 ATOM 매입 거래, 평균 집행가격, 수수료 및 시장영향
- Community Pool Deposited transaction과 누적 귀속액
- Pending/Overdue, 환불·공제·provider payout 후 순기여이익

## 5. v1.1 승인 가능 상태

**OWNER REVIEW READY / CONDITIONAL GO**

v1.1 Candidate는 90일 Discovery 및 제한적 Asset Distribution MVP의 의사결정 문서로 승인 검토가 가능하다. Assured Delivery의 생산 보상운영, Enterprise Gateway의 상업판매, Revenue Vault의 실자금 집행, 대형 native module 개발은 외부 법률검토·실제 수익증거·담보·준비금 게이트 통과 전까지 보류한다.
