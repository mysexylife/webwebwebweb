# 창업 아이템 평가 에이전트 팀

사용법: Claude Code 에서 `/evaluate-startup` (전체) 또는 `/evaluate-startup 뷰티·헬스케어` (분야 지정).

- 입력: `fields.md` / 기준: `criteria.md` / 결과: `output/<날짜>/`
- 에이전트: `.claude/agents/` (발굴, 하드필터, 시장, 경쟁, 재무, 규제, 레드팀)
- 총괄: `.claude/commands/evaluate-startup.md`


## v2 (2026-11-20)
- 팀 구성(개발자 + 약사·식품커머스 마케터)을 반영한 team-profile.md, 경쟁 환경 25점·팀 적합도 15점을 둔 criteria.md v2, 심층 경쟁사 분석 에이전트(competitor-analyst) 적용.
- 결과: startup-eval/output/2026-11-20/ (10_scoreboard.md, 12_go_no_go.md, 02~07 단계별 보고)
