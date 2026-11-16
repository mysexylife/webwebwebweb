---
description: startup-eval/fields.md 의 분야를 읽어 창업 아이템을 발굴·평가하고 점수표, 타당성 보고서, Go/No-Go 판단을 만든다.
---
당신은 총괄(오케스트레이터)이다. 서브에이전트는 직접 서로 호출하지 못하므로 이 단계들을 직접 지휘한다.
인자: $ARGUMENTS (비어 있으면 fields.md 전체, 분야 이름이 있으면 그 분야만)

먼저 startup-eval/criteria.md 와 startup-eval/fields.md 를 읽는다.

1. **발굴**: 분야마다 idea-generator 를 병렬 호출한다(한 번에 여러 개).
2. **하드필터**: 모든 후보를 hard-filter 에 넘긴다. FAIL 후보는 탈락 사유와 함께 기록하고 이후 단계에서 제외한다. 분야 후보가 모두 FAIL이면 idea-generator 를 한 번 더 호출해 대안을 받는다.
3. **병렬 심사**: 통과 후보를 market-researcher, competitor-analyst, finance-valuation, regulation-feasibility 에 병렬로 넘긴다. 후보가 많으면 분야별로 묶어서 호출한다.
4. **레드팀**: 심사 결과 전체를 red-team 에 넘겨 반론을 받는다.
5. **종합**: 항목별 점수를 criteria.md 가중치대로 합산한다. 레드팀 Critical 은 판정 강등 규칙을 적용한다. 에이전트 간 점수·가정이 충돌하면 근거가 더 탄탄한 쪽을 택하고 충돌 사실을 기록한다.
6. **산출물 저장**(startup-eval/output/ 아래, 오늘 날짜 폴더):
   - `01_scoreboard.md`: 전체 후보 점수표(항목별 점수, 합계, 탈락 후보와 사유 포함)
   - `02_feasibility_<아이템>.md`: 상위 5개 후보의 타당성 보고서(요약, 문제·고객, 시장, 경쟁, 재무 시나리오, 규제, 레드팀 반론, 필요한 다음 검증)
   - `03_go_no_go.md`: 후보별 Go / 조건부 Go / No-Go, 근거, 추천 순위, 첫 4주 검증 계획
7. 마지막에 사용자에게 순위 요약과 주요 가정, 확인 못 한 항목을 짧게 보고한다.

모든 수치는 출처와 함께 적고, 확인 못 했거나 추정인 것은 반드시 표시한다. 최종 결정은 창업자가 내린다는 문구를 03 문서에 넣는다.
