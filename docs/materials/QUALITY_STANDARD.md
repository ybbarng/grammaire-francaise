# 학습 자료 품질 기준 (Quality Standard)

이 문서는 `docs/materials/` 하위 모든 학습 자료 파일의 품질 기준을 정의한다.
자료 생성, 수정, 검증 시 이 기준을 따른다.

---

## 1. 구조 (Structure)

모든 파일은 아래 섹션을 **순서대로** 포함해야 한다.

| # | 섹션 | 필수 여부 | 비고 |
|---|------|-----------|------|
| 1 | `# N-M. 제목` | 필수 | 파일 최상단, 번호 + 주제명 |
| 2 | `> 도입 질문` | 필수 | 인용 블록으로 학습 동기 유발 질문 |
| 3 | `## 핵심 개념` | 필수 | 공리/정의를 간결하게 |
| 4 | `## 상세 설명` | 필수 | 번호 매긴 하위 섹션(`### 1. ...`)으로 구성 |
| 5 | `## 예문 모음` | 필수 | 테이블 형식, IPA 발음 포함 |
| 6 | `## 비교: 한국어 / 영어 / 다른 로망스어` | 필수 | 최소 한국어, 영어, 스페인어/이탈리아어 1개 |
| 7 | `## 한국어 화자 주의점` | 필수 | 번호 매긴 리스트 (최소 3개) |
| 8 | `## 어원과 역사` | 권장 | 라틴어 기원, 역사적 변화 등 |
| 9 | `## 핵심 정리` | 필수 | 요약 테이블 또는 흐름도 |
| 10 | `## 연습 문제` | 필수 | 최소 3문제, 정답+해설 필수 |
| 11 | `## 다음 단계` | 필수 | 다음 주제로의 연결 안내 |

### 연습 문제 정답 형식

정답은 `<details>` 접기 방식을 표준으로 한다:

```markdown
**1. 문제 내용**

<details>
<summary>정답 및 해설</summary>

정답과 해설 내용

</details>
```

구분선(`---`) 아래 직접 노출 방식도 허용하지만, `<details>` 방식을 우선한다.

---

## 2. 프랑스어 철자 (French Orthography)

### 2-1. 악센트 (Accents)

프랑스어 단어는 **반드시 올바른 악센트 부호**를 포함해야 한다.

| 부호 | 이름 | 예시 |
|------|------|------|
| é | accent aigu | étudiant, café, passé, composé, présent |
| è | accent grave | très, première, règle, frère, mère |
| ê | accent circonflexe | être, fête, forêt, fenêtre, connaître |
| à | accent grave (a) | à (전치사), là, déjà, voilà |
| â | accent circonflexe (a) | âge, grâce, gâteau, château |
| ù | accent grave (u) | où (의문/관계 부사) |
| û | accent circonflexe (u) | sûr, mûr, dû, coût |
| ô | accent circonflexe (o) | tôt, bientôt, hôpital, côté, rôle |
| î | accent circonflexe (i) | île, dîner, connaître, paraître |
| ï | tréma | naïf, Noël (ë), maïs |
| ç | cédille | français, ça, garçon, leçon, reçu |
| œ | ligature o-e | sœur, cœur, œuf, œuvre, mœurs |

### 2-2. 접속법 반과거 시르콩플렉스

접속법 반과거 3인칭 단수는 **반드시** 시르콩플렉스를 표기한다:

| 동사 | 접속법 반과거 3sg | 주의 |
|------|-------------------|------|
| parler | parlât | ← parla(과거 단순)와 구별 |
| finir | finît | |
| être | fût | ← fut(과거 단순)와 구별 |
| avoir | eût | ← eut(과거 단순)와 구별 |
| venir | vînt | ← vint(과거 단순)와 구별 |
| faire | fît | ← fit(과거 단순)와 구별 |
| pouvoir | pût | ← put(과거 단순)와 구별 |
| savoir | sût | ← sut(과거 단순)와 구별 |
| découvrir | découvrît | |
| obéir | obéît | |

### 2-3. 흔한 실수 목록

아래 단어들은 악센트 누락이 특히 잦다. 검증 시 반드시 확인한다:

```
etudiant → étudiant    etre → être           a (전치사) → à
ou (어디) → où          deja → déjà           francais → français
tres → très             premiere → première   regle → règle
general → général       evenement → événement present → présent
passe → passé           compose → composé     ecole → école
cafe → café             frere → frère         soeur → sœur
probleme → problème     connaitre → connaître grace → grâce
ca → ça                 coeur → cœur          oeuvre → œuvre
gateau → gâteau         arrete → arrêté       fenetre → fenêtre
hopital → hôpital       tot → tôt             role → rôle
```

### 2-4. 악센트 판별 원칙

- **IPA 발음 표기** 내부(`/.../`)의 텍스트는 프랑스어 철자가 아니므로 악센트 대상이 아니다.
- **한국어 설명** 내에서 프랑스어 단어를 인용할 때도 악센트를 표기한다.
- **동사 `a`(avoir 3인칭)와 전치사 `à`를 문맥으로 구분**한다:
  - `Il a un chat.` (avoir → 악센트 없음)
  - `Je vais à Paris.` (전치사 → 악센트 있음)

---

## 3. IPA 발음 표기 (Pronunciation)

### 3-1. 표기 형식

- **슬래시** `/.../`를 사용한다 (대괄호 `[...]` 사용 금지).
- 음절 구분은 점(`.`)으로 한다: `/e.ty.djɑ̃/`
- 리에종은 `‿`로 표기한다: `/le.z‿ɑ̃.fɑ̃/`

### 3-2. IPA 기호 표준

반드시 유니코드 IPA 기호를 사용한다. ASCII 근사 표기는 금지한다.

| 올바른 IPA | 금지 (ASCII) | 음가 |
|------------|-------------|------|
| ʒ | zh | 유성 후치경 마찰음 (je, jour) |
| ʃ | sh | 무성 후치경 마찰음 (chat, chez) |
| ə | uh | 중설 중모음/슈와 (le, de) |
| ɛ | eh | 반개 전설 비원순 모음 (est, père) |
| ɔ | oh | 반개 후설 원순 모음 (port, bonne) |
| ɑ̃ | an/aN | 비모음 (en, an, dans) |
| ɔ̃ | on/oN | 비모음 (on, bon, sont) |
| ɛ̃ | in/iN | 비모음 (in, un, vin) |
| ø | eu (닫힘) | 반폐 전설 원순 모음 (peu, jeu) |
| œ | eu (열림) | 반개 전설 원순 모음 (peur, sœur) |
| ʁ | R, r | 유성 구개수 마찰음 (프랑스어 r) |
| ɥ | y+w | 원순 전설 반모음 (lui, nuit) |
| j | y (반모음) | 경구개 접근음 (yeux, bien) |
| w | w | 순연구개 접근음 (oui, moi) |

### 3-3. 예문 모음 테이블의 IPA

예문 모음 테이블은 다음 컬럼을 포함한다:

```markdown
| 프랑스어 | 발음 (IPA) | 한국어 |
```

모든 예문에 IPA 발음을 제공한다. 접속법 반과거 등 고급 주제에서 예문 형식이 다를 수 있으나(고전체/현대어 비교 등), IPA 발음은 가능한 한 포함한다.

---

## 4. 내용 품질 (Content Quality)

### 4-1. 정확성

- 문법 설명은 정확해야 한다. 불확실한 내용에는 출처나 단서를 명시한다.
- 예문은 문법적으로 올바른 프랑스어여야 한다.
- IPA 발음은 표준 프랑스어(français standard) 발음을 따른다.

### 4-2. 일관성

- 동일 단어/개념은 파일 내에서 동일하게 표기한다.
- 다른 파일과의 상호 참조는 `(참조: N-M 주제명)` 형식으로 한다.

### 4-3. 언어 혼용 금지

- 한국어 설명 중에 영어 단어를 불필요하게 섞지 않는다.
- 영어 비교는 `## 비교` 섹션에서 체계적으로 다룬다.
- 예외: 문법 용어(BANGS 등 기억 약어), 언어학 전문 용어

---

## 5. 검증 체크리스트

자료 생성/수정 후 아래 항목을 모두 확인한다:

- [ ] **구조**: 필수 섹션 11개가 순서대로 존재하는가?
- [ ] **악센트**: 프랑스어 단어에 올바른 악센트가 있는가? (2-3 흔한 실수 목록 확인)
- [ ] **IPA 형식**: 슬래시 `/.../` 사용, 대괄호 `[...]` 사용하지 않았는가?
- [ ] **IPA 기호**: 유니코드 IPA 기호만 사용했는가? (ASCII 근사 없음)
- [ ] **연습 문제**: 최소 3문제, 모든 문제에 정답+해설이 있는가?
- [ ] **예문 IPA**: 예문 모음의 모든 예문에 IPA 발음이 있는가?
- [ ] **상호 참조**: 다른 주제 언급 시 참조 표기가 있는가?
- [ ] **오타**: 프랑스어/한국어 오타가 없는가?
