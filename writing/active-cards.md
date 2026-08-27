# Active Cards — Q3 글쓰기 능동화 카드

> chunk·함정·정형표현·연결사를 **한 파일**에서 4-tier + SRS로 관리하는 통합 카드 시스템.
> **`/write`가 자동 관리한다** — 작문 첨삭 중 chunk 추출·Tier 분류·복습 스케줄을 Claude가 처리.
> 사용자 부담은 "작문 + OK 한 번". (drill처럼 따로 호출하면 안 쓰니까 /write에 통합)

---

## 시스템 정의

### 4-tier (부담 조절)

| Tier | 의미 | 처리 | 분량 |
|------|------|------|------|
| **T1** | 오늘의 적극 학습 | 의식적 반복 + 다음날 워밍업 출제 | 1\~2개 |
| **T2** | 단기 복습 | 워밍업 회전 출제 | 5\~10개 |
| **T3** | 간격 반복 (정착) | SRS 자동 스케줄 | 제한 없음 |
| **T4** | 참조 보관 | 카드만 보관, 능동 학습 X | 제한 없음 |

> 핵심 원칙: **모든 오류 카드화 ≠ 모든 오류 의식 학습.** 매일 N개 나와도 T1으로 올릴 건 **1\~2개만** 선택. 나머지는 카드만 누적.

### 카테고리

| 코드 | 의미 | 예 |
|------|------|-----|
| **chunk** | 써야 할 collocation | en terrasse, prendre une décision |
| **cliché** | 한국어 화자 함정 (회피 패턴) | à la terrasse → en terrasse |
| **formule** | 글의 뼈대 정형표현 | Pour ma part, je pense que… |
| **connecteur** | 연결사 | donc, néanmoins, par ailleurs |

### register (사용역)

| 코드 | 의미 | 사용 분기 |
|------|------|----------|
| **W** | 문어 (écrit) | Q3 글쓰기 |
| **O** | 구어 (oral) | Q4 말하기 |
| **S** | 공유 (both) | Q3 + Q4 |

> Q3 글쓰기는 **W + S** 카드를 사용 (O는 Q4 말하기 분기에서 활성화).

### SRS 간격

1일 → 3일 → 7일 → 14일 → 30일 → 숙달(T4 인지)

### 카드 컬럼

`카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류(있으면) | 등록일 | 다음 복습일 | 사용횟수`

### T1 우선순위 결정 (ROI)

| 우선 | 기준 |
|------|------|
| ⭐⭐⭐ T1 | 같은 세션 2회+ 등장 / 매일 쓰이는 정형 / DELF 채점표 직격 |
| ⭐⭐ T2 | 자주 쓰이나 한 번에 외우기 부담 / 시간 지나면 자연 정착 |
| ⭐ T4 | 단발성 어휘 오류 / 향후 학습으로 자동 해소 예정 |

---

## T1 — 적극 학습 중 (1\~2개)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 등록일 | 다음 복습일 | 사용 |
|---|---|---|---|---|---|---|---|
| grammaire | W | 서사 시제: 배경·묘사·상태=반과거 / 일어난 사건=복합과거 (과거 이야기는 현재형 금지; quand+사건=PC) | "이야기를 미는 사건→PC / 멈춰 묘사→imparfait" · 수동태는 웬만하면 X | (7/19~23 실전 정확; 8/6 워밍업 정확) | 2026-07-18 | 2026-08-20 | 6 |
| grammaire | W | 대명동사(재귀)는 복합과거·반과거에서 조동사 être + 재귀대명사 | je me suis dit / je m'inquiétais / on s'est levé | m'a dit ❌ / m'a inquiétais ❌ (8/6 워밍업·재드릴 정확; 8/7 je me suis couché ✅) | 2026-08-02 | 2026-08-14 | 2 |
| grammaire | S | **조동사는 주어가 결정** (사이 낀 목적어 대명사에 끌리지 말 것); je+대명사+ai/avais 미끄러짐 포함 | je l'ai / j'en avais (je→ai) · **Ils nous ont**(ils→ont) · a·avait는 il/elle/on | je l'a·j'avait ❌ (8/6) / **Ils nous avons ❌ (8/11) → ont** / 재귀 me suis 안전 · 8/7·8/10 번역 무슬립 ✅ | 2026-08-06 | 2026-08-13 | 2 |
| grammaire | S | **조동사·양태동사 뒤=원형 / avoir 뒤=과거분사** (둘째 동사를 활용형으로 쓰지 말 것) | je pouvais le **résoudre** / j'ai **résolu** / je veux **partir** — pouvais/ai + 활용형(résolvais) ❌ | je pouvais le résolvais·le porte ❌ (8/9) / 8/10 워밍업 résolu·pouvais résoudre ✅ | 2026-08-09 | 2026-08-13 | 1 |
| grammaire | S | **복합과거 조동사 être** = 위치(A→B)·상태 변화 자동사 + 모든 재귀 (rester 예외) — **자동사≠être** | il est parti/resté/arrivé/tombé / je me suis levé — 단 courir·marcher·nager·dormir·vivre = **avoir** | il a resté·a parti ❌ (8/10) → **드릴 99/100 정착** / 8/13 a dormi ✅ | 2026-08-10 | 2026-08-16 | 2 |
| grammaire | S | **간접화법 시제 일치** (과거 주절→종속절 뒤로): 현재→**반과거**/미래→**조건법**/과거→**대과거** · **시간부사도 backshift** · (단독 서술은 복합과거↔반과거 관점차, 둘 다 가능) | qu'il **mentait** / s'il **viendrait le lendemain** / qu'il **était parti** | qu'il a menti ❌(8/13·8/21·8/23 재발) → **8/23 완전 소화**: 동시=반과거/이전=대과거 자유선택 + 복합과거 금지 규칙 스스로 정리 · 자유작문서 serait·parlaient·parlais ✅ | 2026-08-13 | 2026-08-28 | 4 |
| grammaire | S | **de + 관사** 디폴트=관사(du/des/de la); **무관사는 6가지만**: ①부정 ②양·용기 ③합성머리명사(cours/prof de X) ④관용구 ⑤소유격/지시사 ⑥고유명사 · **⚠️경계: 부정 무관사는 직접목적어 부분관사만** (venir de·부정문이어도 관사 유지) | vient des hormones / ne vient pas des hormones(관사 유지!) / du manque de communication | 8/20 du café ✅ / 8/23 워밍업 ne viennent pas des hormones·mais du cerveau·de l'argent ✅ (경계 습득) | 2026-08-18 | 2026-08-28 | 3 |
| grammaire | S | 도시(무관사 de Paris)↔나라(관사 du Japon/des USA; 여성국가만 de France 생략) · jouer **de**+악기(du piano/de la guitare) | de Paris ↔ du Japon / je joue du piano | de Japon ❌ / 8/21 est venu du Brésil↔à Lyon·née au Portugal↔à Madrid ✅ | 2026-08-18 | 2026-08-26 | 1 |
| grammaire | S | **monter/descendre/sortir/rentrer/passer/retourner + 목적어 → avoir** (없으면 être) | il est monté ↔ il **a** monté les valises / passer un examen=avoir | 목적어 있으면 avoir 함정 — 8/10 드릴 ✅ / 8/21·8/23 a monté les valises ✅ | 2026-08-10 | 2026-08-28 | 3 |
| cliché | S | **connaître**(사람·장소·경험으로 앎) ≠ **savoir**(사실·방법·정보) · 사람 몰랐던 **상태**=connaissait(반과거) | je connais Paris/le restaurant / je sais que…, je sais nager | savait le restaurant ❌ (8/21) / 8/21·8/23 워밍업 je connais cette ville·cet homme / ne sais pas où·son nom ✅ — **사용자 요청 특별관리** | 2026-08-21 | 2026-08-27 | 2 |
| cliché | S | **jouer à**(게임하다·놀다) ≠ **jouir de**(향유하다; 단독 jouir=성적 함의 조심) · **jouer de**+악기 | il a joué aux jeux vidéo / jouer à Overwatch / jouer du piano — jouir de la vie(누리다) | a joui au jeu vidéo ❌ (8/21) → a joué / 8/23 워밍업 재발 joue les jeux vidéo·au piano ❌ → 재생산서 du violon·aux cartes ✅ | 2026-08-21 | 2026-08-26 | 1 |
| grammaire | S | **동사 + de/à + 원형** (전치사 값은 동사마다 고정): décider **de** · essayer **de** · réussir **à** · commencer **à** · apprendre **à** · continuer à · choisir de | j'ai décidé **de** commencer **à** étudier | ❌ ×5 (8/23) "버릇 안 듦" → 8/25 워밍업 décider de·arrêter de·commencer à·réussir à·envie de 전부 ✅ (엘리지옹 d'arrêter만) | 2026-08-23 | 2026-08-28 | 1 |
| grammaire | S | **demander/ordonner à qqn de + 원형** (~에게 ~하라고 시키다) ≠ commander qch à qn(주문하다) · à+les=**aux** | j'ai demandé **à** l'IA **de** créer / **aux** étudiants de se taire | commandé l'IA à créer ❌ (8/23) → 8/25 demandé aux étudiants de se taire·lui ai demandé de fermer ✅ (à les→aux만) | 2026-08-23 | 2026-08-28 | 1 |

## T2 — 단기 복습 (5\~10개)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 등록일 | 다음 복습일 | 사용 |
|---|---|---|---|---|---|---|---|
| chunk | W | 감정 형용사 + de + 부정사 (Je suis heureux/content/fier de…) | 감정=사람 주어+être+de (de=감정의 원인·출처). 다른 주어면 que+접속법 | C'est heureux ❌ / de être → d'être | 2026-07-13 | 2026-07-18 | 3 |
| formule | S | **soit** = 즉·다시 말해 (= c'est-à-dire) — **등가 치환**(soit 뒤엔 같은 값만, 비교 long comme X). 철자 soit(≠sois 접속법) | 90 minutes, soit une heure et demie | 8/24 massed 2/2 ✅ / 8/27 soit long comme △·sois ❌ → soit toute la matinée·une heure et demie ✅ | 2026-08-24 | 2026-08-28 | 2 |
| grammaire | S | 지시형용사 **ce**(남자음)/**cet**(남+모음·무음h)/**cette**(여) — 발음상 cet=cette 동일 주의 | ce livre / **cet** homme·examen / **cette** ville | cet ville ❌(8/23) / Ce examen ❌(8/27) → cet examen (둘 다 자가검출 ✅) | 2026-08-27 | 2026-08-28 | 0 |
| chunk | S | **il (m')a fallu + 기간 + `pour` + 원형** (~하는 데 걸리다) ≠ il faut + 원형(해야 한다) | Il m'a fallu une semaine pour développer / cinq ans pour parler couramment (=ça m'a pris) | pour 누락·pendant ❌ → 8/24·8/25 massed ✅ / 8/25 pour 재확인 ✅ (ans≠années) | 2026-08-24 | 2026-08-28 | 2 |
| cliché | S | 회사 = l'entreprise (travailler dans / mon·notre entreprise) | bureau≠회사 / notre l'entreprise ❌ | mon bureau(회사) ❌ | 2026-07-15 | 2026-07-19 | 3 |
| cliché | S | informer qqn ≠ communiquer/annoncer qch | 사람에게 알리다 / 결정을 통보하다 | la décision soit informé ❌ → communiquée | 2026-07-16 | 2026-07-17 | 0 |
| grammaire | W | il aurait mieux valu + 부정사 | ~하는 게 나았을 것이다 | il aurait fait mieux annoncer ❌ | 2026-07-16 | 2026-07-17 | 0 |
| cliché | S | Ce qui m'a frappé/étonné (me=직접목적어, être 없음) | frapper/étonner qqn 능동 | ce qui m'a été frappé ❌ → m'a frappé | 2026-07-18 | 2026-07-19 | 0 |
| chunk | S | être en rupture de stock | 품절이다 | toujours rare (덜 자연) | 2026-07-18 | 2026-07-19 | 0 |
| cliché | S | chaque + 단수명사 ↔ chacun(단독) | 각각의 ~ (chaque magasin) | du chacun magasin ❌ | 2026-07-18 | 2026-07-19 | 0 |
| grammaire | W | 예정된 과거 = devait + 부정사 (~할 예정이었다) | 조건법(serait)·조건법과거(aurait été) 아님 — imparfait de devoir | la cérémonie serait organisé ❌ → devait avoir lieu | 2026-07-19 | 2026-07-23 | 1 |
| cliché | S | le cours(수업, 남) ≠ la cour(마당, 여) | 철자·성으로 뜻 바뀜 | la cours(수업) ❌ | 2026-07-19 | 2026-07-20 | 0 |
| cliché | S | 요일 앞 무전치사 (avoir lieu samedi / lundi prochain) | 요일엔 à/le 없이 바로 | avoir lieu à samedi ❌ | 2026-07-20 | 2026-07-21 | 0 |
| grammaire | W | 대명사 y = à + 사물/장소 | j'y pense(penser à) / je m'y entraîne(s'entraîner à) | me l'entraîner ❌ | 2026-07-20 | 2026-07-21 | 0 |
| grammaire | W | séparer A **de** B | A와 B를 분리하다 (et 아님) | séparer vie pro et vie privée ❌ | 2026-07-21 | 2026-07-22 | 0 |
| grammaire | W | se contrôler (자기 통제) | 통제하다는 대상 필요; 자기 자신=se contrôler | contrôler soi-même ❌ (7/28 워밍업 정확) | 2026-07-24 | 2026-07-30 | 1 |
| grammaire | W | 소유형용사는 주어에 일치 (il→son/ses, ils→leur/leurs) | 복수 주어면 leur/leurs | Ils…son rôle ❌ → leur | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | de + le/les = du/des (축약) | de+le=du, de+les=des | de les personnes ❌ → des | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | aider qqn à + 부정사 | ~하도록 돕다 (주어 다르면 à로 연결, pour X) | aider pour ne pas perdre ❌ → à | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | dire que (≠ parler que) · **dire는 목적어 필요**(무엇을: dire la vérité) / parler **de**(~에 대해) | dire la vérité(parler ❌) / parler de ses problèmes | 8/23 재발 On parle 99 ❌→dit / 8/27 il m'a dit la vérité·parler de ses problèmes ✅ | 2026-08-11 | 2026-08-30 | 3 |
| cliché | S | étrange(이상한) ≠ étranger(외국인·외국의) | 철자로 뜻 바뀜 | les étranges ❌ → les étrangers | 2026-07-25 | 2026-07-26 | 0 |
| chunk | S | avoir du mal **à** + 부정사 (전치사 à!) · avoir de la peine **à**도 à (de ❌) | ~하기 힘들다 (avoir mal à=아프다와 구별) | avoir mal à courir ❌ (7/28 워밍업 정확) / 8/21 peine **de** ❌→à (자가 미검출) | 2026-07-27 | 2026-08-22 | 1 |
| grammaire | W | partir(자동사, 목적어 X) ↔ quitter(타동사) ↔ sortir de | 떠나다(그냥) / ~을 떠나다(quitter+avoir) / ~에서 나가다(sortir de+être) | Il est parti la chambre ❌ | 2026-07-28 | 2026-07-29 | 0 |
| chunk | W | s'efforcer de + 부정사 / retenir ses larmes | 애쓰다 / 눈물을 참다 | (잘 씀) | 2026-07-28 | 2026-07-29 | 0 |
| chunk | S | faire semblant de + 부정사 | ~인 척하다 (comme si de rien n'était 사촌) | (7/31 massed 3맥락 정착) | 2026-07-31 | 2026-08-01 | 0 |
| grammaire | S | arriver = être (il est arrivé) | 이동·발생 자동사 = être | il a arrivé ❌ | 2026-08-02 | 2026-08-03 | 0 |
| grammaire | W | s'arrêter de + 부정사 / se transformer en | ~하기를 멈추다 / ~로 변하다 | arrêter prendre ❌ / transformer le rideau ❌ | 2026-08-02 | 2026-08-03 | 0 |
| chunk | S | faire d'une pierre deux coups | 일석이조 | (잘 씀 8/2, 굳히기) | 2026-08-02 | 2026-08-03 | 0 |
| grammaire | W | 주어 같으면 que+접속법 대신 부정사 | Je souhaite/espère **pouvoir** (que je puisse ❌) — 주어 다르면 que+접속법 | souhaite que je puisse ❌ | 2026-08-02 | 2026-08-03 | 0 |
| grammaire | W | assister à qch / croire à qch → y | ~을 목격하다 / ~을 믿다(y로 받음) | assister le dragon ❌ / je n'croyais ❌ | 2026-08-02 | 2026-08-03 | 0 |
| cliché | S | entendre(들리다) ≠ écouter(경청) · emmener(데려가다) ≠ entraîner | hear≠listen / 사람 데려가다=emmener | entendre l'explication △ / nous a entraîné ❌ | 2026-08-02 | 2026-08-03 | 0 |
| grammaire | W | croire à qch → y (en 아님) | j'y crois / je n'y croyais pas | je n'en croyais ❌ | 2026-08-03 | 2026-08-04 | 0 |
| grammaire | W | 재귀 성수일치: se=직목→일치 / se=간목→무일치 | 무일치 목록: se parler·dire·téléphoner·demander·rendre compte 등; 기본은 일치 | s'est transformé ❌→transformée / s'est dite ❌(dit 고정) | 2026-08-03 | 2026-08-04 | 0 |
| grammaire | W | **복수 주어/선행사 → 복수 동사** (수 일치) | les nouvelles disparaissent / qui agitent | est partagé·agite·disparaît ❌ (8/6 워밍업 정확) | 2026-08-04 | 2026-08-09 | 1 |
| grammaire | W | **on = 동사 3인칭 단수** (과거분사·형용사만 복수 일치) | on se dispute / on est arrivés(과거분사만) | on se bagarrons·connaissions ❌ (8/6 워밍업 정확) | 2026-08-04 | 2026-08-09 | 1 |
| grammaire | W | être + 과거분사 → 주어 성수일치 (수동·대명·이동 통합; avoir 무일치) | sont partagées / a été invitée | est partagé ❌ | 2026-08-04 | 2026-08-05 | 0 |
| cliché | S | 구별 동사: parler/dire·exprimer(구조) · entendre/écouter(의미) | 한국어가 합친 것 | parler son opinion ❌ → exprimer | 2026-08-04 | 2026-08-05 | 0 |
| chunk | S | tenir sa promesse | 약속을 지키다 (tenir: il tient) | tien se promesse ❌ → tient sa | 2026-07-31 | 2026-08-01 | 0 |
| grammaire | W | 빈도부사(toujours/souvent/rarement/jamais)는 활용 동사 직후 | Il tient toujours sa promesse | 문장 끝 ❌ | 2026-07-31 | 2026-08-01 | 0 |
| cliché | S | connaître(사람·장소 알다) ≠ savoir(사실 알다) | me connaître / savoir que | ne me savait pas ❌ → connaissait | 2026-07-31 | 2026-08-01 | 0 |
| chunk | S | faire de son mieux | 최선을 다하다 | je fais meilure ❌ (재확인) | 2026-07-27 | 2026-08-01 | 1 |
| chunk | S | sans s'en rendre compte (주어별: m'en/t'en/s'en/nous en/vous en) | 자기도 모르게 (뿌리=se rendre compte de qch 깨닫다) | sans connaissance ❌ / 주어 se 변화 누락 | 2026-07-21 | 2026-07-26 | 11 |
| grammaire | W | devenir/venir/… = être 보조 (복합과거) | elle est devenue (+ 일치) | a devenu ❌ → est devenue | 2026-07-15 | 2026-07-16 | 0 |
| cliché | S | un média (남성, 복수 les médias) | 매체 | les nombreuses médias ❌ → nombreux | 2026-07-15 | 2026-07-16 | 0 |
| chunk | S | être en (bonne/mauvaise) forme | 컨디션이 좋다/나쁘다 | avoir mauvaise forme ❌ | 2026-07-15 | 2026-07-16 | 0 |
| cliché | S | 직업·직책은 무관사 (elle est rédactrice / PM) | être + 직업 (un/une 생략) | un rédactrice ❌ | 2026-07-15 | 2026-07-16 | 0 |
| grammaire | W | 동사 + 전치사 (à/de/sur…; sur+명사) | aller **à** / s'inscrire **à** / se concentrer **sur** / essayer de / rêver de / décider de / apprendre à | 8/9 전치사 누락 3건 ❌ / 8/10 워밍업 s'inscrire au·se concentrer sur ✅ | 2026-07-08 | 2026-08-13 | 4 |
| grammaire | W | depuis + 기간 + 현재 (~한 지 ~째) | J'apprends depuis 3 ans (지속) | il y a 3 ans(=~전) 혼동 | 2026-07-13 | 2026-07-14 | 0 |
| cliché | S | on dit que (사람들이 ~라고 한다) | ~라고들 한다 | on parle que ❌ | 2026-07-13 | 2026-07-14 | 0 |
| cliché | S | à + 도시 (무관사) | ~에 (도시) | au Paris ❌ → à Paris | 2026-07-13 | 2026-07-14 | 0 |
| grammaire | W | 엘리지옹 = 모음/무음h **앞에서만** (자음 앞엔 절대 X) | l'/d'/qu'/j'/n'/s'/c'/m'/t' · 자음 앞은 la/le/de 그대로 | 8/11 재발 → 당일 재드릴 ✅ → **8/13 자유 유지 ✅**(s'il·qu'il·c'est) | 2026-07-07 | 2026-08-16 | 10 |
| chunk | S | petit à petit / peu à peu | 조금씩 | peu un peu ❌ | 2026-07-08 | 2026-07-09 | 0 |
| formule | W | il n'y a pas de meilleur(e) X que Y | Y보다 나은 X는 없다 | ce n'est la meilleure méthode que ❌ | 2026-07-08 | 2026-07-09 | 0 |
| chunk | S | faire les accords / lire les partitions | 코드를 잡다 / 악보를 읽다 | attraper l'accord ❌ (calque) | 2026-07-08 | 2026-07-09 | 0 |
| grammaire | W | ce qui(주어) ↔ ce que(목적어) | "~하는 것" — Ce qui + 동사, c'est + 명사 / ce que + 주어+동사 | C'est important qui… ❌ (선행사 없음) / ce que influence ❌ | 2026-07-06 | 2026-07-09 | 1 |
| chunk | S | s'entraîner à + 부정사 / travailler qch(직접) | 연습·훈련하다 (s'entraîner **à** viser / travailler sa visée) | exerciser ❌ / s'entraîner sa visée ❌ (8/7) / 8/8~9 à viser·à le résoudre·je m'entraînais ✅ | 2026-07-07 | 2026-08-12 | 2 |
| chunk | S | faire des progrès en + 언어 | ~ 실력이 늘다 | de compétence pour ❌ (calque) | 2026-07-07 | 2026-07-08 | 0 |
| cliché | S | facilement (부사) ≠ facile (형용사) | 동사 수식은 부사 | français facile ❌ / facile séparer ❌ (재발 7/21) | 2026-07-07 | 2026-07-22 | 0 |
| chunk | W | c'est/il est + 형용사 + de + 부정사 | "~하는 것은 ~하다" (절 X, 부정사 O) | c'est facile qu'on arrive ❌ → d'arriver | 2026-07-05 | 2026-07-12 | 2 |
| chunk | S | être bon pour la santé | 건강에 좋다 | fait en bonne santé ❌ (직역) | 2026-07-06 | 2026-07-07 | 0 |
| chunk | S | une alimentation variée / des nutriments | 균형 잡힌 식단 / 영양소 | la nourritures ❌ / la riche nutrition | 2026-07-06 | 2026-07-07 | 0 |
| cliché | S | basé sur (not de) | ~에 기반한 | basé de ❌ | 2026-07-06 | 2026-07-07 | 0 |
| cliché | S | une horloge (여성) / le rythme biologique | 생체시계 | un horloge ❌ | 2026-07-06 | 2026-07-07 | 0 |
| chunk | S | ranger (정리하다) | (물건·방을) 정리 (ranger sa chambre) | arranger ❌ (재발 7/27) | 2026-07-03 | 2026-07-28 | 2 |
| chunk | S | en voiture / en train (교통수단) | 교통수단 = en + 무관사 | avec voiture ❌ → en voiture | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | profiter de | ~을 즐기다·누리다 | jouir le soleil ❌ → profiter du | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | se souvenir de / un souvenir | 기억하다 / 추억 | le memoire ❌ (=기억력·논문) | 2026-07-05 | 2026-07-06 | 0 |
| cliché | S | les vacances (항상 여성 복수) | 휴가 (de nouvelles vacances) | la nouvelle vacance ❌ | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | commander (주문하다) | 음식·물건 주문하다 | ordré ❌ (영어 order) | 2026-07-02 | 2026-07-06 | 2 |
| chunk | W | après s'être + p.p. (재귀 부정사과거) | "~한 후에" 재귀동사 (재귀대명사 유지) | après être réveillé ❌ → m'être | 2026-07-02 | 2026-07-06 | 3 |
| cliché | S | nouveau(앞)/nouvel(모음앞)/nouvelle(여) ↔ neuf(뒤, 신품) | un nouvel ordinateur / un ordinateur neuf | un neuf ordinateur ❌ | 2026-07-03 | 2026-07-12 | 1 |
| cliché | S | cette chambre (chambre 여성) | 방 (la chambre) | ce chambre ❌ | 2026-07-03 | 2026-07-04 | 0 |
| cliché | W | avoir + 앞 직목(que·le/la/les) → 과거분사 일치 (en·간목 lui는 무일치) | que j'ai achetées / je les ai écrites / je l'ai jouée | que j'ai monté ❌ / 8/7 je les ai écrites·je l'ai jouée·elle l'y a travaillée ✅ | 2026-07-03 | 2026-08-14 | 2 |
| chunk | W | après + avoir/être + p.p. (infinitif passé) | "~한 후에" (주절보다 선행, être면 주어 일치) | après passer ❌ / Après j'ai appris ❌ (8/9) / 8/10 워밍업 après avoir appris ✅ | 2026-06-24 | 2026-08-13 | 6 |
| cliché | W | 재귀동사 복합과거 일치: se=COD→일치 / se=COI→무일치 | s'est lavée vs s'est lavé les mains / se sont parlé(à) / 본질재귀=주어일치, 예외 s'est rendu compte | "재귀=무조건 일치" 과잉일반화 | 2026-06-24 | 2026-07-05 | 3 |
| grammaire | W | quand + 미래시제 (futur) | "~할 때"(미래)는 불어는 futur | quand j'ai ❌ → j'aurai (7/3 워밍업 오답 → 작문서 정확) | 2026-07-02 | 2026-07-05 | 1 |
| chunk | S | s'entraîner à + 동사원형 | ~하는 걸 연습하다 | s'entraîner que ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | S | 형용사 후치 (petit-déjeuner tardif) | 대부분 형용사는 명사 뒤 | le tard petit-déjeuner ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | W | peu de + 가산복수 (몇 개 안 남음) | il reste peu d'épisodes | un peu de episodes reste ❌ | 2026-07-02 | 2026-07-03 | 0 |
| chunk | S | l'application de livraison | 배달 앱 | delivery app ❌ (영어) | 2026-07-02 | 2026-07-06 | 1 |
| chunk | S | il y a quelques années | 몇 년 전에 | quelque ans ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | S | en ville (무관사) ↔ dans la/cette ville (특정) | 일반 "도시에"=en ville / 특정 도시=dans+관사 | en cette ville ❌ (재발, en은 무관사) | 2026-06-23 | 2026-06-27 | 2 |
| chunk | W | beaucoup de + 무관사 (+ 복수면 동사 복수) | 많은 ~ (de l'argent ❌ → d'argent) | des tas de / beaucoup de l'argent / 동사 단수 ❌ | 2026-06-23 | 2026-06-25 | 1 |
| chunk | S | arriver à / dans (+ 전치사) | ~에 도착하다 | arriver la rue ❌ | 2026-06-24 | 2026-06-25 | 0 |
| chunk | S | rentrer chez soi | 귀가하다 | je vais chez moi (덜 자연) | 2026-06-24 | 2026-06-25 | 0 |
| chunk | S | sur le/mon chemin | 가는 길에 | dans mon chemin ❌ | 2026-06-24 | 2026-06-25 | 0 |
| cliché | S | prendre le déjeuner / déjeuner(동사) | 식사하다 (점심=déjeuner, 아침=petit-déjeuner) | manger le déjeuner ❌ / petit-déjeuner(아침) 혼동 | 2026-06-24 | 2026-06-25 | 0 |
| cliché | S | campagne(시골) ≠ compagne(동반자) | 철자로 뜻 바뀜 | à la compagne ❌ | 2026-06-22 | 2026-06-26 | 1 |
| cliché | S | même si + 직설법 | 양보 "설령 ~라도" | même s'il soit ❌ → est | 2026-06-22 | 2026-06-26 | 1 |
| chunk | W | en + 제롱디프 (주어 일치) | ~하면서 (en me déplaçant) | en se déplaçant ❌ (je 주어) | 2026-06-23 | 2026-06-24 | 0 |
| chunk | S | un embouteillage / embouteillé | 교통체증 / (도로가) 막힌 | "막히다" 미상 | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | le reste(나머지) ≠ les restes(남은 음식) | 단/복수로 뜻 바뀜 | les restes ❌ | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | la santé (여성) | 건강 | mon santé ❌ → ma | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | place → endroit / lieu | 장소 (place=광장·자리) | place 오용 | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | chercher → trouver / aller | 찾다 ≠ 가다·이용 | chercher 남용 | 2026-06-22 | 2026-06-25 | 0 |
| chunk | W | tout ce dont / ce que | ~하는 (모든) 것 | 관계대명사 누락 | 2026-06-22 | 2026-06-25 | 0 |
| connecteur | W | Premièrement / Deuxièmement / Enfin | 첫째/둘째/마지막 | En premier·seconde ❌ | 2026-06-22 | 2026-07-08 | 1 |
| chunk | S | transports en commun | 대중교통 | La transport ❌ / des tas de transport ❌ | 2026-06-22 | 2026-06-26 | 1 |
| cliché | S | S'il (엘리지옹) | Si + il → S'il | Si il ❌ (재발) | 2026-06-22 | 2026-06-25 | 0 |
| chunk | W | préférer A plutôt que B | A를 B보다 선호 | plus vivre que ❌ / plutôt que à → qu'à | 2026-06-22 | 2026-07-08 | 1 |
| chunk | S | **jouer à + 게임** (→ 대명사 y) ↔ **jouer + 캐릭터**(직접목적어 → le/la 성일치) | jouer à Overwatch / y jouer ↔ jouer Ana → je l'ai jouée | jouer Overwatch·Nous l'avons joué ❌ (8/7 재발) / 8/8 워밍업 jouer à Overwatch·j'ai joué Ana ✅ | 2026-06-22 | 2026-08-12 | 2 |
| chunk | W | un entraînement à l'écriture | 작문 훈련 | s'exercer 작문 ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | pour progresser | 실력을 늘리려고 | — | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | quelque chose (불변 단수) | 무언가 | quelque choses ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | un personnage de soutien | 서포터 (게임 역할) | l'assistant position ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | soigner ses coéquipiers | 팀원을 치료하다 | récupérer la forme ❌ | 2026-06-22 | 2026-06-25 | 0 |
| formule | S | Ce qui me séduit, c'est… | 내가 매력 느끼는 건 ~ (강조 분열문) | que je suis charmé ❌ | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | utiliser (not utilize) / on peut | 사용하다 / 활용 | 영어혼용 + on peux | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | en dehors de | ~밖에·외부에 | dehors Buzzvil ❌ | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | chercher sur Internet | 인터넷에서 검색하다 | rechercher l'internet ❌ | 2026-06-22 | 2026-06-25 | 0 |
| formule | S | Je veux dire… / C'est dommage | 내 말은~ / 아쉽다 | (잘 씀, 강화) | 2026-06-22 | 2026-06-25 | 0 |
| grammaire | S | **en → 과거분사 무일치** (앞 직목처럼 보여도 X) | j'en ai lu deux/quelques-uns (lu 불변) · 대조 le/les는 일치(je les ai lus) | j'en ai lus ❌ (8/6) / 8/7 j'en ai lu trois ✅ | 2026-08-06 | 2026-08-10 | 1 |
| grammaire | S | le/la/les(특정·한정) ↔ en(불특정·비한정 양) | 그 케이크 je le mange / 케이크 좀·불특정 j'en mange (다 먹어도 불특정이면 en) | 특정↔부분 혼동 / 8/7 je les ai écrites·j'en ai lu ✅ | 2026-08-06 | 2026-08-10 | 1 |
| grammaire | S | y = 장소 전치사구(à/dans/sur/en/chez+장소)→거기 / de+장소→en | j'y vais(dans/à/chez) ↔ j'en viens(de) | dans/chez 장소 미대명사화 / 8/7 je n'y suis pas allé ✅ | 2026-08-06 | 2026-08-10 | 1 |
| grammaire | S | demander/ordonner qch **à** qqn → lui (COI, 무일치) | 사람=간접목적어 lui/leur (l' 아님) | je ne l'ai ordonnée ❌ → je ne lui ai … ordonné (8/6) | 2026-08-06 | 2026-08-07 | 0 |
| grammaire | S | c'était/on était + 요일 (il était ❌) | 요일·날짜는 ce/on; il est는 시각(il est 3h) | il était mercredi △ | 2026-08-06 | 2026-08-07 | 0 |
| formule | W | C'était la première fois que + 반과거 | ~한 건 처음이었다 | mon premier pas que ❌ | 2026-08-06 | 2026-08-07 | 0 |
| cliché | S | **parmi** (셋 이상 중에서) ≠ **entre** (둘 사이) | parmi les héros / entre toi et moi | Entre les héros ❌ → Parmi (8/7) / 8/8 Parmi ✅ | 2026-08-07 | 2026-08-12 | 1 |
| cliché | S | **créer**(만들다) ≠ **crier**(외치다) | elle a créé une partie / il a crié | elle a crié une partie ❌ (8/7) / 8/8 a créé ✅ | 2026-08-07 | 2026-08-12 | 1 |
| grammaire | S | 과거 사실=복합과거; **aller + 과거분사 ❌** (futur proche는 aller + 부정사) | nous avons gagné (과거) / nous allons gagner (곧) | nous allons gagné ❌ (8/7) / 8/8 nous avons gagné ✅ | 2026-08-07 | 2026-08-12 | 1 |
| cliché | S | 온라인 **café ❌ → forum / communauté** (콩글리시 faux-ami) | s'inscrire à un forum / une communauté en ligne | un café de Rubik's cube ❌ (8/9) / 8/10 forum ✅ | 2026-08-09 | 2026-08-13 | 1 |
| grammaire | S | se dire **que**(서술) ↔ se demander **si**(의문); se demander = **재귀+être**(s'est demandé, 무일치) | Je me **suis** demandé si… (se·est 빠뜨리지 말 것) | 8/18 재발: J'ai demandé(se 빠짐)·Il se demandé(est 빠짐) → me suis demandé | 2026-08-09 | 2026-08-19 | 1 |
| grammaire | W | la possibilité / il est possible **que** + **접속법** | je laisse ouverte la possibilité que nous **soyons** | possibilité que nous **sommes** ❌ (8/18) → soyons | 2026-08-18 | 2026-08-19 | 0 |
| grammaire | W | (se) comparer **à** (목적어 필요); **à+사람=à lui 강세형 유지**(재귀+à사람은 클리틱 X) | se comparer au passé / à lui (je me le suis comparé ❌) | comparer avec le passé ❌(8/18) / 8/20 à lui ✅ | 2026-08-18 | 2026-08-23 | 1 |
| grammaire | W | 습관·일반 과거 = **반과거** (대과거는 "더 이전"일 때만) | on se réjouissait des récoltes / on chassait | avait joui·avait réussi(습관인데 대과거) ❌ (8/18) | 2026-08-18 | 2026-08-19 | 0 |
| grammaire | W | **비인칭 가주어 il/c'est**: 뒤에 **동사만**(de+원형 / que+접속법절), **명사 못 옴**, **불변 단수** | il est important de faire / que tu fasses | ce sont importants que + 명사 ❌ (8/18) / 8/20 Il est important de dormir ✅ | 2026-08-18 | 2026-08-23 | 1 |
| grammaire | W | **명사 생략 = 지시대명사** celui(남단)/celle(여단)/**ceux**(남복)/celles(여복) + pour/de/qui | à celles pour les avancés / à **ceux** pour adultes(exercices 남복) | aux pour ❌ (8/18) / 8/20 à ceux ✅ | 2026-08-18 | 2026-08-23 | 1 |
| grammaire | W | **강조 mise en relief**: 강조 대상=**주어→qui** / 비주어→**que** · 긴 명사 주어 미루기=**의사분열문 Ce qui est important, ce sont [명사]** | Ce sont X et Y **qui** sont importantes / C'est pour… **que** … | qui/que 혼동(8/18) / 8/20 Ce qui est important, ce sont… ✅ | 2026-08-18 | 2026-08-23 | 1 |
| grammaire | W | **pour que + 접속법**(주어 다름) ↔ **pour + 원형**(주어 같음) | pour qu'on résolve…, la mémorisation est importante(주어 다름 ✅) | 같은 주어에 pour que ❌ | 2026-08-18 | 2026-08-19 | 0 |
| grammaire | S | interdire **à** qqn **de** + 부정사 (= ~에게 ~을 금지하다) | il m'interdisait de résoudre / m'a interdit de sortir / lui a interdit de boire / nous ont interdit d'entrer | il prohibait me résoudre ❌ (8/9) / 8/11 massed 4회(me/lui/nous) ✅ | 2026-08-09 | 2026-08-14 | 1 |
| grammaire | S | au lieu de + 명사/원형 (de+사람=**de lui**) · de+사물=en / de+사람=de lui/elle | au lieu de lui / au lieu de partir — en은 사물·불특정 양만 | Eric en a travaillé au lieu ❌ (8/10) / 8/11 au lieu de le faire ✅ | 2026-08-10 | 2026-08-14 | 1 |
| grammaire | S | **comme si**(마치~인 듯, 반사실) ↔ **comme / de même que**(실제 비교) | comme s'il dormait(실제 X) / comme lorsqu'on interdit…(실제 O) | comme si on interdit(운전 중 금지=실제) ❌ (8/11) → comme lorsqu'on — 논리 뒤집힘 | 2026-08-11 | 2026-08-12 | 0 |
| grammaire | S | avoir le droit **de** + 원형 (à ❌) | ils ont le droit de choisir / de jouer / de poser des questions | le droit à utiliser ❌ (8/11); 8/13 "모르겠어" → 재학습·재생산 4회 ✅ | 2026-08-11 | 2026-08-16 | 2 |
| grammaire | S | distraire / déranger qqn = **직접목적어**(le/la/les, leur ❌) | qch qui les distrait | qui leur distraient ❌ (8/11) → les distrait | 2026-08-11 | 2026-08-12 | 0 |

## T3 — 간격 반복 (정착)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 정착일 | 다음 복습일 | 단계 |
|---|---|---|---|---|---|---|---|
| grammaire | W | comme si + 반과거(현재 비현실)/대과거(과거 비현실) | comme s'il était millionnaire / comme si j'avais gagné · 대과거 aux 주의(rencontrer=avoir) | 8/11 재발 → 당일 재드릴 ✅ → **8/13 자유작문 유지 ✅**(comme s'il avait compris) 자동화 다리 형성 | 2026-08-11 | 2026-08-16 | 2일 |
| grammaire | W | comme si de rien n'était(관용, se 없음·n'était) / comme s'il ne s'était rien passé(se passer 대과거, il 고정) | 아무 일도 없었던 것처럼 | de rien s'était ❌ / il 누락 (7/28 자유 인출 2회 정착) | 2026-07-28 | 2026-07-31 | 3일 |
| grammaire | W | **comme si + 대과거 형성** (avait + 과거분사) — active 되돌림 | comme s'il n'avait rien su/vu/entendu (부정사 X, 과거분사 O; ne...rien) | comme s'il n'a rien entendu ❌(PC 금지) (8/6 워밍업 정확·이유 설명) | 2026-08-03 | 2026-08-09 | 3일 |

## T4 — 참조 보관 (능동 학습 X)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 발견일 | 비고 |
|---|---|---|---|---|---|---|
| cliché | S | insectes (not insects) | 곤충 | 영어 혼용 | 2026-06-22 | 단발 |
| chunk | S | se déplacer | 이동하다 | (자연 표현) | 2026-06-22 | 참조 |
| chunk | S | tout près | 바로 가까이 | (자연 표현) | 2026-06-22 | 참조 |
| cliché | S | le français (남성) | 프랑스어 | la français ❌ | 2026-06-23 | 향후 자동 해소 |
| cliché | S | populaire (not popular) | 인기 있는/대중적 | popular ❌ (영어 혼용) | 2026-06-24 | 단발 |
| chunk | S | une rue gourmande / des restaurants | 맛집 거리 | rue de goût ❌ | 2026-06-24 | 참조 |
| chunk | S | le sirop d'érable | 메이플 시럽 | maple syrop ❌ (영어) | 2026-07-02 | 단발 |
| chunk | S | monter / assembler (un meuble), une vis / un boulon | 가구 조립 / 나사·볼트 | 조립·볼트 (한국어) | 2026-07-02 | 참조 |
| chunk | S | cette nuit / ce soir | 오늘 밤 / 오늘 저녁 | dans la nuit d'aujourd'hui ❌ | 2026-07-03 | 참조 |
| chunk | S | le grand large | 넓은 바다·먼바다 | le grand monde ❌ (=사교계) | 2026-07-05 | 참조 |
| cliché | S | large (넓은) ≠ 영어 large(큰) | 큰=grand / 넓은=large | faux-ami (large=크다 오해) | 2026-07-05 | 참조 |
| chunk | S | les hormones / le système immunitaire | 호르몬 / 면역계 | hormones de l'immunité (어색) | 2026-07-06 | 참조 |
| chunk | S | surfer sur les vagues | 파도를 타다 | surfer sur le mouvement ❌ | 2026-07-05 | 참조 |
| chunk | S | grimper / monter (une montagne) | (산을) 오르다 | assensionner ❌ (없는 말) | 2026-07-05 | 참조 |
| chunk | S | un système d'alerte de stock | 재고 알림 시스템 | système d'alarme ❌ | 2026-07-18 | 참조 |
| chunk | S | un magasin physique | 오프라인 매장 | magasin hors ligne ❌ (calque) | 2026-07-18 | 참조 |
| chunk | S | la détaxe / un jour férié | 면세 / 공휴일 | détaxé ❌ | 2026-07-18 | 참조 |
| cliché | S | une console (여성) | 게임기 | il est (console) ❌ → elle | 2026-07-18 | 참조 |
| chunk | S | une navette (du campus) | 순환 셔틀버스 | bus circulaire ❌ | 2026-07-19 | 참조 |
| chunk | S | une résidence universitaire | (대학) 기숙사 | pension universitaire ❌ | 2026-07-19 | 참조 |
| chunk | S | en bas ↔ en haut | 아래쪽 ↔ 위쪽 | la bas/la haut ❌ | 2026-07-19 | 참조 |
| chunk | S | avoir l'impression de + 부정사 | ~한 기분이 들다 | avoir l'air d'être un coup de poing ❌ | 2026-07-19 | 참조 |
| cliché | S | un parapluie (남성) | 우산 | la parapluie ❌ | 2026-07-20 | 참조 |
| cliché | S | difficulté (이중 f) | 어려움 | dificulté ❌ | 2026-07-20 | 참조 |
| cliché | S | le moral / le bien-être (≠ la mentalité) | 정신 건강·기분 | mieux pour ma mentalité ❌ | 2026-07-21 | 참조 |
| cliché | S | bleu (철자) / le ciel bleu | 파란 | blue ❌ (영어) | 2026-07-21 | 참조 |
| cliché | S | une attente (기대) ≠ attendre (기다리다) | les attentes des autres | l'attendre d'autre ❌ | 2026-07-24 | 참조 |
| cliché | S | indéfiniment (무한정) | 계속·끝없이 | infinitement ❌ | 2026-07-24 | 참조 |
| cliché | S | une fonction / une fonctionnalité (여성) | 기능 | le nouvel fonction ❌ → une nouvelle | 2026-07-25 | 참조 |
| chunk | S | les réseaux sociaux (un réseau social) | SNS·소셜 미디어 (≠ les médias 매체) | (단어 미상) | 2026-07-25 | 참조 |
| chunk | W | balbutier quelques mots | 몇 마디 더듬거리다 | (잘 씀, 고급) | 2026-07-25 | 참조 |
| chunk | S | avoir l'air de + 부정사 / + 형용사 | ~해 보이다 (il a l'air de dormir / fatigué) | (잘 씀) | 2026-07-27 | 참조 |
| grammaire | W | 부사 bien은 부정사 앞 (bien peindre) | 어순 | peindre bien ❌ | 2026-07-27 | 참조 |
| grammaire | S | passer(지나가다)=être (il est passé) | 자동사 이동 = être (partir/sortir처럼) | il a passé ❌ | 2026-07-31 | 참조 |
| chunk | S | une aurore boréale / une éclipse solaire totale | 오로라 / 개기일식 | — | 2026-08-02 | 참조 |
| chunk | S | un long temps de pose / un casque de VR / la pollution lumineuse / des arbres enneigés | 긴 노출 / VR 헤드셋 / 광공해 / 눈 덮인 나무 | — | 2026-08-02 | 참조 |
| cliché | S | dormir(자다, 재귀 X) ≠ s'endormir(잠들다, 재귀) | faire semblant de dormir | se dormir ❌ | 2026-07-31 | 참조 |
| chunk | S | de suite / d'affilée (연달아) ↔ successivement(격식·차례로) | gagner plusieurs matchs de suite | successivement △ (딱딱) | 2026-08-07 | 참조 |
| chunk | S | viser / la visée / une partie personnalisée | 조준하다 / 조준 / 사용자 지정 게임 | (게임 어휘) | 2026-08-07 | 참조 |
| cliché | S | un cubeur / une cubeuse (≠ cubiste) | 큐브 푸는 사람 (cubiste=입체파 화가, faux-ami) | cubists ❌ / cubiste(콩글리시) | 2026-08-09 | 참조 |
| chunk | S | occupé(e) à + 부정사 (~하느라 바쁘다) | j'avais les mains occupées à le résoudre | mains occupé à s'entraîner ❌ | 2026-08-09 | 참조 |
| chunk | S | en présentiel / une rencontre / chronométrer | 대면으로 / 모임 / 시간을 재다 | hors ligne ❌(calque) / mesurer un record △ | 2026-08-09 | 참조 |
| cliché | S | résoudre (철자 — résou**dre**, r 하나) | 풀다·해결하다 | résourdre ❌ (고질, 8/9 ×5) | 2026-08-09 | 참조 |
| grammaire | S | tout 남성복수 = **tous** (touts ❌) / 여성복수 toutes | je les ai tous/toutes 과거분사 | touts ❌ (8/10 자가교정) | 2026-08-10 | 참조 |
| chunk | S | tomber dans l'escalier / le matin(아침에) | 계단에서 넘어지다 / 아침에 (au matin 문어 △) | sur escalier ❌ / au matin △ | 2026-08-10 | 참조 |
| chunk | S | un lieu d'apprentissage / d'apprendre ❌ | 배움의 장 (lieu de + 명사) | un lieu d'apprendre ❌ | 2026-08-11 | 참조 |
| chunk | S | pendant la récréation / avec modération / tout le temps | 쉬는 시간에 / 절제하며 / 항상(tous les temps ❌) | par exemple la récréation(전치사 누락) / tous les temps ❌ | 2026-08-11 | 참조 |
| grammaire | S | 일반 "그것은 + 형용사" = **ce**(c'était/c'est), il은 특정 남성명사만 | que ce n'était pas important | qu'il n'était pas important △ (막연한 그것) | 2026-08-11 | 참조 |

---

## Q4 대비 — 구어 "phrases de survie" (register O · Q3 미활성)

> Q4 말하기 분기에서 활성화. 8/3 ChatGPT 음성 대화 후 사용자 요청 — 막혔을 때 대화를 끊지 않고 이어가는 생존 표현.

| reg | 표현 | 뜻 |
|---|---|---|
| O | Vous pouvez répéter, s'il vous plaît ? | 다시 말해 주시겠어요? |
| O | Plus lentement, s'il vous plaît. | 조금 천천히요. |
| O | Comment dit-on … en français ? | ~를 프랑스어로 뭐라고 해요? |
| O | Je ne sais pas comment le dire. / Je n'arrive pas à l'expliquer. | 어떻게 말할지 모르겠어요 / 설명을 못 하겠어요 |
| O | Attendez, je réfléchis. | 잠깐만요, 생각 중이에요. |
| O | Qu'est-ce que ça veut dire ? | 그게 무슨 뜻이에요? |

---

## 사전 풀 (Q3 시작 시 베이스라인 자가 분류 → T1\~T4 배치)

> 5/1 작문 시범 결과 + 핵심 정형표현. Q3 시작 시 사용자가 "이미 능동/반복 필요/모름"으로 자가 분류하면 그게 베이스라인이 되고, 카드가 T1\~T4로 흩어진다.

### chunk (collocation)

| reg | 표현 | 의미 | 흔한 오류 |
|---|---|---|---|
| S | en terrasse | 카페 야외석에 | ~~à la terrasse~~ ⭐ 5/1 큰 수확 |
| S | prendre une décision | 결정을 내리다 | ~~faire une décision~~ |
| S | faire la queue | 줄을 서다 | |
| S | prendre une photo | 사진을 찍다 | |
| S | passer un examen | 시험을 보다 | ~~voir un examen~~ |
| S | tomber dans les pommes | 기절하다 | (단발성 → T4 후보) |

### cliché (한국어 화자 함정) — 5/1 시범 13개

| reg | 정답/회피 | 함정 | 비고 |
|---|---|---|---|
| S | offrir (호의·선물) | ~~donner~~ | ⭐⭐ 한 세션 2회 등장 — T1 1순위 |
| S | donner/raconter qch **à qqn** | 수령자 누락 | "주다/말하다" 직역 |
| S | depuis(지속) ↔ il y a(시점) | 혼동 | 시간 표현 핵심 |
| S | son + 모음명사 | ~~sa + 모음~~ | 발음 hiatus 회피 |
| W/S | en + gérondif / pendant + 명사 | ~~pendant + 동사원형~~ | 강한 직역 함정 |
| S | 명사 직접 목적어 | l'histoire de… 풀어쓰기 | "X의 이야기" → "X" |
| S | arriver / être servi (음식) | ~~sortir~~ | 동사 선택 |
| S | personnage / thé / heure | character / téa / hour | 영어 혼용 → T4 |
| W | avec X écrit dessus | qui est écrit… | 관계절 어색 구조 |

### formule (정형표현 6카테고리)

| reg | 표현 | 기능 |
|---|---|---|
| W | Pour ma part, je pense que… | 의견 |
| S | Il me semble que… | 인상 |
| W | Cela dit, … | 양보 |
| S | En revanche, … | 대조 |
| W | En somme, … | 요약 |
| S | Ce qui m'intéresse, c'est… | 강조 |
| S | Ça fait + 기간 + que + 절 | "~한 지 ~됐다" ⭐ 5/1 수확 |

### connecteur (연결사)

| reg | 표현 | 단계 |
|---|---|---|
| S | donc / alors | A2\~B1 |
| W | en effet / par ailleurs | B1\~B2 |
| W | néanmoins / cependant | B1\~B2 |
| W | en dépit de / faute de | C1 |

---

## 통계 (주 1회 /write 자동 산출)

> 신규 chunk 수 / Tier 이동(T2→T3 정착) / 활용 빈도 / 활용 미달(사용 권장) 등.
> **회사 공유 = 매달 1,500단어 (양적만, 6/22 확정).** 질적(rubric DELF B1 6항목)·chunk는 **내부 측정/방향타 도구** (회사 공유 X).
