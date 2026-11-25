# 팀프로젝트 산출물 목록 | 야간 침실 모기 요격 시뮬레이션

산출물 목록 · 작성 gm(초안 보조 Codex) · 검토 gm 예정 · 상태 초안 · v0.5 · 개정일 2026-11-25

| 일차 | ID | 산출물 | 실무 명칭 | 스테이지 | 책임자 | 검토자 | 상태 | 버전 | 관련 ID | 작업 파일 경로 |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | D02 | 팀 차터 | Project Charter | 01 | gm · PM | gm 예정 | 초안 | v0.5 | D01, D03 | [차터](../charter/charter.md) |
| 1 | — | 산출물 목록 | Deliverables Register | 01 | gm · PM | gm 예정 | 초안 | v0.5 | D01~D08 | [산출물 목록](register.md) |
| 2 | D01 | 문제 정의서 | Problem Statement | 01 | gm · PM | gm 예정 | 초안 · 검토 대기 | v0.5 | D02, D03 | [문제 정의서](../problem-statement/problem-statement.md) |
| 3 | D03 | 요구사항 명세 | PRD / SRS | 02 | gm · PM | gm 예정 | 초안 · 검토 대기 | v0.6 | R-01~R-10 | [요구사항 명세](../requirements/requirements.md) |
| 4 | D06 | 시스템 구조·인터페이스 | System Architecture / ICD | 03 | gm · 설계 | gm 예정 | 초안 · 검토 대기 | v0.2 | R-01~R-07 | [시스템 구조](../architecture/architecture.md) |
| 4 | D07 | 장면 구성표 | BOM 대응 | 03 | gm · 시뮬레이션 | gm 예정 | 초안 · 검토 대기 | v0.3 | R-01, R-02, R-04~R-07 | [장면 구성표](../scene-inventory/scene-inventory.md) |
| 4 | D08 | 안전 개념 | Safety Concept | 03 | gm · 시뮬레이션 | gm 예정 | 초안 · 검토 대기 | v0.2 | R-02, R-04~R-06 | [안전 개념](../safety-concept/safety-concept.md) |
| 4 | 장면 v0 | MJCF, 스크린샷, 확인 출력 | MuJoCo 장면 | 03 | gm · 시뮬레이션 | gm 예정 | 로컬 장면 실행 확인 · 제출 자료 준비 대기 | 로컬 `clearance` | D07, D08 | [D07 장면 구성표](../scene-inventory/scene-inventory.md) |
| 5 | D04 | 테스트 시나리오·추적표 | Traceability Matrix | 02 | gm · QA | gm 예정 | 초안 · 검토 대기 | v0.4 | R-01~R-10 / T-01~T-09 | [테스트 계획](../test-plan/test-plan.md) |
| 5 | D05 | 일정·작업 분해·위험 목록 | Project Plan / Risk Register | 02 | gm · PM | gm 예정 | 초안 · 검토 대기 | v0.3 | D02~D04 | [일정·위험 목록](../schedule-risks/schedule-risks.md) |

## 1일차 저장소와 실행 환경

- [공유 문서 저장소](https://github.com/mosquito-swatter-robolab/docs)의 기준 브랜치는 `main`이다.
- 실험 절차와 결과는 [D04 테스트 추적표](../test-plan/test-plan.md)와 [실험 근거](../evidence/README.md)에서 확인한다.
- 실행 당시 환경은 Windows, Python 3.12.14, MuJoCo 4.0.1이었다.

| 팀원 | OS | 설치 결과 | 장면 열기 결과 | 기록 위치 또는 남은 문제 |
|---|---|---|---|---|
| gm | Windows | 기존 가상환경에서 실행 확인. 새 환경 설치 재현 대기 | 액추에이터 24개와 자유도 24개를 로드했다. 시드 `410042`는 293틱에 유효 포획, 최소 이격 66.7 mm, 접촉·한계 위반 0건을 기록했다. | [410042 재생 기록](../evidence/pillow-clearance-410042.json) · [100시드 요약](../evidence/README.md#동일-시드-100개-비교) · GUI 확인 대기 |

100개 시드 비교에서 진입 전 포획 35회, 보호 구역 진입 36회, 미결 29회였다. 보호 구역 접촉·팔 간 접촉·동작 한계 위반은 각각 0건이었다. 내부 목표는 진입 31회 이하이며 강한 포충등의 진입은 32회였다. 강의 인수 기준은 미정이다. [비교 실험 기록](../evidence/README.md#동일-시드-100개-비교) · [시드별 결과](../evidence/bedroom-comparison.csv)

1일차 제출 항목은 차터, 산출물 목록, 공유 저장소 주소다. 2~5일차 초안도 네 팔 침실 실험을 반영했다. 시험 절차와 로컬 결과는 D04에서 확인한다.
