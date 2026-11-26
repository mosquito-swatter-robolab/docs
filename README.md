# Mosquito Swatter RoboLab

문서 v0.1 · 개정일 2026-11-25

잠든 사람 곁으로 모기가 날아올 때, 침대 주위의 로봇 팔 네 대가 사람에게 닿지 않고 모기를 먼저 잡을 수 있을까요? 컴퓨터 안에 침실을 만들고 같은 100가지 시작 조건에서 장치가 없을 때, 포충등을 켰을 때, 로봇을 썼을 때를 비교했습니다. MuJoCo는 그 안에서 물체의 움직임과 접촉을 계산하는 프로그램입니다.

처음이라면 [사용자의 문제](problem-statement/problem-statement.md) → [어느 결과면 성공인가](requirements/requirements.md) → [시험 결과](test-plan/test-plan.md) 순서로 읽으세요. 서쪽 팔 배치를 바꾼 뒤 모기의 진입은 36회에서 29회로 줄어 내부 목표인 31회 이하를 충족했습니다. 같은 팔의 부품끼리 충돌하고 관절 속도와 가속도가 한계를 넘어 안전 시험은 미달입니다.

## 문서 목록

| 일차 | 문서 | 작성 양식 | 강의 제출 항목 |
|---|---|---|---|
| 1 | [D02 팀 차터 v0.6](charter/charter.md) | [양식](charter/template.md) | `docs/charter.md` |
| 1 | [산출물 목록 v0.6](register/register.md) | [양식](register/template.md) | `docs/register.md`, 공유 저장소 주소 |
| 2 | [D01 문제 정의서 v0.6](problem-statement/problem-statement.md) | [양식](problem-statement/template.md) | `docs/problem.md` |
| 3 | [D03 요구사항 명세 v0.7](requirements/requirements.md) | [양식](requirements/template.md) | `docs/requirements.md`, `tests/test_judge.py`, `src/judge.py` |
| 4 | [D06 시스템 구조 v0.3](architecture/architecture.md) | [양식](architecture/template.md) | `docs/architecture.md` |
| 4 | [D07 장면 구성표 v0.5](docs/scene.md) | [양식](scene-inventory/template.md) | [장면 XML](scenes/bedroom-v0.xml), [스크린샷](scenes/bedroom-v0.png), [확인 출력](scenes/bedroom-v0-check.json) |
| 4 | [D08 안전 개념 v0.3](safety-concept/safety-concept.md) | [양식](safety-concept/template.md) | `docs/architecture.md`에 D06과 함께 제출 |
| 5 | [D04 테스트 시나리오·추적표 v0.5](test-plan/test-plan.md) | [양식](test-plan/template.md) | 3일차 추적표 예시 참고 |
| 5 | [D05 일정·위험 목록 v0.4](schedule-risks/schedule-risks.md) | [양식](schedule-risks/template.md) | 1일차 산출물 목록 참고 |

1~5일차 초안은 UR10e 네 대를 사용한 침실 실험을 반영했습니다. D04의 시험 ID는 D03의 요구사항과 연결됩니다.

## 실험 근거

100시드 비교, 머리맡 410042 재생, 진입 후 36회 진단은 이 저장소에서 확인할 수 있습니다. [실험 기록과 데이터](evidence/README.md)

## 문서 개정 방법

이 저장소의 문서를 개정할 때는 현재 파일을 같은 폴더의 `문서명-v현재버전.md`로 먼저 이름 변경한다. 보관한 본문을 복사해 원래 파일명으로 새 현재본을 만들고, 변경 내용과 새 버전·개정일을 기록한다. 예를 들어 D03 v0.4는 `requirements-v0.4.md`에 보관하고 v0.5는 `requirements.md`에서 편집한다.

보관본은 원문 그대로 유지한다. 개정 후 아래 이력과 산출물 목록의 버전을 맞춘다. 현재본 링크는 기본 파일명으로, 특정 시점의 판정 근거는 해당 버전 파일명으로 연결한다.

## 이전 버전

- 팀 차터 · [v0.3](charter/charter-v0.3.md)
- 산출물 목록 · [v0.2](register/register-v0.2.md) · [v0.3](register/register-v0.3.md) · [v0.4](register/register-v0.4.md)
- 문제 정의서 · [v0.3](problem-statement/problem-statement-v0.3.md) · [v0.4](problem-statement/problem-statement-v0.4.md)
- 요구사항 명세 · [v0.2](requirements/requirements-v0.2.md) · [v0.3](requirements/requirements-v0.3.md) · [v0.4](requirements/requirements-v0.4.md) · [v0.5](requirements/requirements-v0.5.md)
- 테스트 추적표 · [v0.3](test-plan/test-plan-v0.3.md)

### 이번 개정 직전 문서

- 사람이 겪는 불편 · [직전 문서 v0.5](problem-statement/problem-statement-v0.5.md) · [직전 양식](problem-statement/template-v0.0.md)
- 팀이 확인하려는 것 · [직전 문서 v0.5](charter/charter-v0.5.md) · [직전 양식](charter/template-v0.0.md)
- 필요한 문서 찾기 · [직전 문서 v0.5](register/register-v0.5.md) · [직전 양식](register/template-v0.0.md)
- 성공을 판단하는 두 질문 · [직전 문서 v0.6](requirements/requirements-v0.6.md) · [직전 양식](requirements/template-v0.0.md)
- 시험 결과 읽기 · [직전 문서 v0.4](test-plan/test-plan-v0.4.md) · [직전 양식](test-plan/template-v0.0.md)
- 남은 일과 시작 조건 · [직전 문서 v0.3](schedule-risks/schedule-risks-v0.3.md) · [직전 양식](schedule-risks/template-v0.0.md)
- 모기 한 마리를 발견하면 · [직전 문서 v0.2](architecture/architecture-v0.2.md) · [직전 양식](architecture/template-v0.0.md)
- 침실 장면 둘러보기 · [직전 문서 v0.3](scene-inventory/scene-inventory-v0.3.md) · [직전 양식](scene-inventory/template-v0.0.md)
- 팔은 언제 멈춰야 하나 · [직전 문서 v0.2](safety-concept/safety-concept-v0.2.md) · [직전 양식](safety-concept/template-v0.0.md)

이전에 자체 버전이 없던 안내문과 양식은 처음 보관한 원본을 v0.0으로 표시합니다. [이전 첫 화면](README-v0.0.md) · [이전 실험 안내](evidence/README-v0.0.md)
