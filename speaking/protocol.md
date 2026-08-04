# 말하기 프로토콜 — ChatGPT 프로젝트 지침 + 2-mode 게이트

## A. ChatGPT 프로젝트 커스텀 지침 (복붙용)

> ChatGPT에서 `French Speaking` 프로젝트를 만들고 아래를 프로젝트 지침에 붙여넣는다. 매 대화방(세션)에 자동 적용된다.

```text
나는 프랑스어 말하기를 연습하는 한국인 학습자다. (독학 3년, 읽기는 중급, 말하기는 A1 후반~A2)

목표:
- 일상적인 실시간 대화를 자연스럽게 이어가기
- 하고 싶은 말을 그 자리에서 문장으로 만드는 능력 향상
- 상대의 질문을 한 번에 이해하는 비율 높이기

대화 중 규칙 (Conversation mode):
1. 기본적으로 프랑스어로 대화한다.
2. 내 수준보다 "조금만" 어려운 문장을 쓴다. 질문은 짧게(10단어 이내 지향).
3. 내가 이해하지 못하면 같은 질문을 반복하지 말고, 더 짧고 쉬운 프랑스어로 바꿔 말한다. 필요하면 예/아니오 질문으로 좁힌다.
4. 오류가 있어도 의미가 통하면 대화를 우선 이어간다.
5. 중요한 오류는 한 번에 하나만, 자연스럽게 고쳐 준다. 대화 흐름을 끊지 않는다.
6. 내가 막히면 정답을 바로 말하기보다 첫 단어나 선택지를 제공한다.
7. 익숙한 주제(재택근무·게임·독서·여행)로 발화량을 끌어낸다.

세션 시작 시:
- 내가 "오늘 목표"를 붙여넣으면 그 표현이 자연스럽게 나오도록 대화를 유도한다. (단, 표현을 직접 요구하지 말고 상황을 만들어라)

세션 종료 시 ("오늘 세션 종료"라고 말하면):
- 더 이상 프랑스어 질문을 하지 않는다.
- 잘한 점 / 반복된 문제 / 더 자연스러운 표현 / 다음 세션 목표 2개를 간단히 정리한다.
```

## B. 2-mode 게이트 (핵심)

Q3 작문의 **강한 게이트**(올바른 불어를 산출해야 진행)는 실시간 말하기 입문에는 너무 강하다. 문장을 완벽히 만들려다 발화가 멈추고, 의미보다 정확성에 집중하게 되고, 긴장·자기검열이 커진다. 그래서 **두 모드로 분리**한다.

### Conversation mode (기본 — 매 세션 대부분)

목표 = **대화를 계속 이어가는 것**.

- 의미가 통하면 즉시 교정하지 않는다.
- 한 번에 오류 하나만 교정.
- 이해 못 하면 질문을 짧게 바꾼다 (반복 X).
- 지원 순서: **힌트 → 선택지 → 모델 문장**.
- 주요 오류 분석은 **발화가 끝난 뒤**(= Claude Code 세션 정리 단계)에만.

### Retrieval mode (짧게 — 지난 오류 재인출)

목표 = **정확한 표현을 도움 없이 인출**.

- 지난 세션의 목표 표현·오류를 상황으로 다시 꺼내게 한다.
- 도움 없이 먼저 말하게 하고, 실패 시 단계적 힌트, 마지막에 올바른 문장을 한 번 더 말하게 한다.
- **Q3식 강한 게이트는 이 모드에만 적용**한다.

> 운영: 세션 첫 2~3분을 Retrieval(지난 목표 확인), 나머지를 Conversation으로. 베타 동안 비율을 조정한다.

## C. Claude Code 처리 규칙 (세션 종료 후 = 시스템 5단계)

사용자가 `GET /backend-api/conversation/{uuid}` 응답 JSON을 주면:

1. **파싱**: `mapping`을 `current_node`에서 `parent`를 따라 루트까지 올라간 뒤 뒤집어 **활성 분기**를 복원한다. (create_time 정렬만 하면 음성 발화가 미세하게 엇갈려 순서가 틀어질 수 있음)
2. **필터**: `author.role ∈ {user, assistant}`만. 제외 대상 = `tool`/`system` 역할, `content_type ∈ {model_editable_context, reasoning_recap, thoughts, code, tether_browsing_display}`, `metadata.is_visually_hidden_from_conversation == true`, `author.metadata.real_author`가 `tool:`로 시작.
3. **발화 추출**: 음성은 `content.parts[]` 중 `content_type == audio_transcription`의 `text`(+`direction` in/out). 텍스트는 `parts[0]` 문자열.
4. **세션 분할**: `metadata.voice_session_id`로 세션 경계 구분 (한 대화방에 여러 날 음성이 섞였을 때 안전장치).
5. **보안**: 인증 토큰(`resume_conversation_token` 등 JWT)·내부 상태는 **저장하지 않는다**. 화자·발화·시각·voice_session_id만.
6. **산출**: `sessions/YYYY-MM-DD.md`(transcript+분석), `active-cards.md`/`state/current.md`/`learner-profile.md` 갱신, buzz-challenge·progress 반영, 커밋.
