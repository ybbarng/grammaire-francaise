# Français Grammaire — 대화형 프랑스어 문법 학습

## 프로젝트 목적
1. 프랑스어 문법을 A1부터 C2(문어체 포함)까지 완벽히 체계적으로 학습
2. 프랑스어 문장을 자유롭게 구사할 수 있는 수준 도달

## 학습 방식
- **웹앱 아님** — Claude와 대화형으로 수업 + 피드백
- 정형화된 퀴즈보다 **설명 → 연습 → 교정** 흐름
- `docs/notion-export/` 에 기존 ChatGPT와 정리한 문법 자료 있음 (Notion export)

## 언어 전환 전략
- Phase 1 (A1-A2 복습): 한국어로 설명, 예문만 프랑스어
- Phase 2 (B1-B2): 간단한 프랑스어 + 한국어 보조
- Phase 3 (C1+): 프랑스어 위주, 모르는 부분만 한국어
- 사용자가 프랑스어로 시도하면 적극적으로 프랑스어로 응답

## 슬래시 커맨드
사용자는 아래 커맨드로 세션을 관리한다. 각 커맨드의 상세 절차는 `.claude/commands/` 참고.

- `/project:study` — 학습 세션 시작 (진도 확인 → Notion 자료 참고 → 수업)
- `/project:review` — 취약점 복습
- `/project:write` — 작문 연습
- `/project:end` — 세션 종료 (세션 기록 작성 → progress.md 업데이트 → 커밋)

## 커밋 규칙
- 커밋은 `/project:end` 실행 시에만 한다.
- 커밋 메시지 형식: `학습: [주제명] - 간단 요약` / `복습: ...` / `작문: ...`
- 스테이징 대상: `progress.md`, `sessions/`, `exercises/`

## 진도 추적
- `progress.md`에 전체 커리큘럼 진도표가 있다 (항목별 상태, 이해도, 마지막 학습일).
- `sessions/YYYY-MM-DD.md`에 세션별 상세 기록이 있다.
- 커리큘럼 상세 목록은 `progress.md` 참고.

## 파일 구조
- `CLAUDE.md` — 이 파일. 프로젝트 컨텍스트 및 규칙
- `progress.md` — 커리큘럼 진도표 + 취약점 메모
- `sessions/` — 세션별 상세 기록
- `exercises/` — 작문 연습 및 교정 기록
- `docs/notion-export/` — Notion에서 가져온 기존 문법 자료
- `.claude/commands/` — 슬래시 커맨드 정의
