# Mosquito Swatter RoboLab

MuJoCo로 모기 요격 로봇을 실험하는 프로젝트의 문서 저장소입니다.

## 문서 목록

| 일차 | 문서 | 작성 양식 | 강의 제출 항목 |
|---|---|---|---|
| 1 | [D02 팀 차터 v0.5](charter/charter.md) | [양식](charter/template.md) | `docs/charter.md` |
| 1 | [산출물 목록 v0.5](register/register.md) | [양식](register/template.md) | `docs/register.md`, 공유 저장소 주소 |
| 2 | [D01 문제 정의서 v0.5](problem-statement/problem-statement.md) | [양식](problem-statement/template.md) | `docs/problem.md` |
| 3 | [D03 요구사항 명세 v0.6](requirements/requirements.md) | [양식](requirements/template.md) | `docs/requirements.md`, `tests/test_judge.py`, `src/judge.py` |
| 4 | [D06 시스템 구조 v0.2](architecture/architecture.md) | [양식](architecture/template.md) | `docs/architecture.md` |
| 4 | [D07 장면 구성표 v0.3](scene-inventory/scene-inventory.md) | [양식](scene-inventory/template.md) | `docs/scene.md`, `scenes/*.xml`, 장면 스크린샷, 확인 코드 출력 |
| 4 | [D08 안전 개념 v0.2](safety-concept/safety-concept.md) | [양식](safety-concept/template.md) | `docs/architecture.md`에 D06과 함께 제출 |
| 5 | [D04 테스트 시나리오·추적표 v0.4](test-plan/test-plan.md) | [양식](test-plan/template.md) | 3일차 추적표 예시 참고 |
| 5 | [D05 일정·위험 목록 v0.3](schedule-risks/schedule-risks.md) | [양식](schedule-risks/template.md) | 1일차 산출물 목록 참고 |

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
